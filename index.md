# Peyton's User Page

![M](PagePic.JPG)
## Personal Life
Hello my name is **Peyton Gaudet** and I am currently in my first year at UCSD after transferring from a community college in the Sacramento area. I am a computer science major and I was able to end up with a 3.92 GPA at my community college and received 4 associates degrees. 

I am all about working hard to acheive my goals. A quote that resonates with me is:
>You can't get much done in life if you only work on the days when you feel good." - Jerry West.

I really like this quote because it is easy to work your way towards your goals when you are in the mood for it. However, the people that set themselves apart from the rest are the ones that put in consistent work on a daily basis, no matter the circumstances.

As you can see, that quote was from Jerry West, an all-time great Laker, and I chose that quote because I am a huge Lakers fan. Also, in my picture I am wearing a Raiders sweatshirt so sports are a huge part of my life as you can tell. I played baseball and basketball in high school and I regularly play basketball and go to the gym. 

## Programming Life 

As a programmer, I have accrued practical experience through many years of coding. I have a good understanding of:

- Python
- Java
- C++
- Julia
  
Most of my personal projects are made in Python like my sports betting arbitrage bot and my stock market trading bot. Through coursework, I was able to get a solid foundational knowledge of C++ and Java. I was prepared well by my community college *(Sierra College)* to be able to be successful in my courses at UCSD. Before going to UCSD this year, I was somewhat nervous. I felt like everyone had a step up on me but I have gained confidence after completing a few upper division courses there. I was able to work hard and be really successful in my courses thus far. I have also taken a couple of course outside of my schooling in Machine Learning and Web Development. My ideal career paths in order would be:
1. Machine Learning Engineer
2. Cybersecurity Analyst
3. Web Development

I have always been good at math and I want to be able to make good money coming out of college without doing many years of schooling so computer science seemed like the most logical option for me. I enjoy problem solving and being powerful behind a computer. I want to be extremely knowledgeable about the devices that have taken over our world.

Last quarter, I learned how to implement K-Means clustering in Julia! Here is a code snippet that implemented my own K-Means algorithm.
```
function k_means(X, K, max_iter)
    n, d = size(X)
    centroids = X[randperm(n)[1:K], :]
    clusters = zeros(Int64, n)
    for i in 1:max_iter
        # Assign each data point to the closest cluster
        for j in 1:n
            distances = [norm(X[j,:] - centroids[k,:]) for k in 1:K]
            clusters[j] = argmin(distances)
        end
        # Update centroids of each cluster
        for k in 1:K
            idx = findall(clusters .== k)
            if length(idx) > 0
                centroids[k,:] = mean(X[idx,:], dims=1)
            end
        end
    end
    return clusters, centroids
end
```
This is the one of the first steps to learn about how unsupervised machine learning algorithms work. I was able to give a lecture on K-Means clustering in a Jupyter notebook which was really cool.


My future goals include: 
- [ ]  Landing an internship
- [ ]  Improve on my stock market bot using machine learning
- [ ]  Being financially stable


To get back to the personal life section click this [link](#personal-life)!

Here is a [picture](kobe-bryant-wallpapers-hd-2015-wallpaper-cave-2-800x800.jpg) to my favorite basektabll player of all time. (*This should not be a surprise :)*

Here is a [link](https://chat.openai.com/chat) to ChatGPT that I beleive will truly change the way that people interact with technology. I hope to be working on the NLP algorithms in the future because they are an exciting step in our advancement as humans!