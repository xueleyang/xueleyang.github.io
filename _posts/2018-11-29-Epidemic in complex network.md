---
layout:     post
title:      Epidemic in complex network
subtitle:  what do, how do(advatange, disadvantage), what can I do, critical thinking  
date:       2018-11-29
author:     LeyangX
header-img: img/post-bg-desk.jpg
catalog: 	 true
tags:
    - Epidemic process
---


# Summary about SI, SIR, SIS

## SI

*  model
*  result

## SIS

 * model
 * result

## SIR

> this is reference 
Epidemic processes in complex networks

![Figure1](https://cl.ly/33ccfe1b47a5)

***

# code

`def data_average(user_degree,rs,n):
​    log_user_degree = np.log(user_degree)
​    process_user_degree = list(map(lambda x: round(x,n), log_user_degree))
​    x = np.sort(list(set(process_user_degree)))
​    L=[]
​    for each in x:
​        L.append(np.average(rs[np.where(process_user_degree == each)[0]]))
​    return np.array(x), np.array(L)`