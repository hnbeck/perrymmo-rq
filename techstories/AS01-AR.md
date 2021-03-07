# Assumption about AR

## Technical state

AR devices will be available in 2021 and following years. As far as known today, most AR devices use Unity for rendering and working with DotNet (C#). This is true for NREAL glasses and also Qculus products. Unity is based on C#. With MonoGame, there is a simple GameEngine available in C# which allows easier implementation of graphics for the first step than Unity. 

With .Net 6  and .Net this technology is complete plattform independed and has a lot of libraries and technical infrastructure, including books and other ressources. 

As a runtime, .Net allows other languages to use, especially F# for functional programming. Logic programming is only available by miniKanren. There is now useful Prolog implementation available for .Net. 

## Conclusion

The nodes shall be coded as .Net product, using miniKanren for the logic part. 


## Questions

It may be possible to port a Prolog like GNU Prolog to .Net. 
