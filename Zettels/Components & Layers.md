***

A *component* is a part of [[System|system]] in charge of a single job, coupling to the *system* by using an [[Interface|interface]].
To avoid ***recursive complexity***, we abstract *components* up to the point in which they are a *black box* for which we only care about its ***function*** and ***interface***.  


A *layer* is a group of *components* with a shared purpose. It's characterized by the strict ***one-way dependency*** rule, which states that a *layer* doesn't need to know anything about the next one, but it depends heavily on the previous *layer*.

***