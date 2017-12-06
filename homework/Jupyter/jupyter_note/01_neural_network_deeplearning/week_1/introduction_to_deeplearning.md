
# Coursera | Andrew Ng （01-week-1 ）—Introduction to Deep Learning
深度学习概论

    该系列仅在原课程基础上部分知识点添加个人学习笔记，或相关推导补充等。如有错误，还请批评指教。在学习了 Andrew Ng 课程的基础上，为了更方便的查阅复习，将其整理成文字。因本人一直在学习英语，所以该系列以英文为主，同时也建议读者以英文为主，中文辅助，以便后期进阶时，为学习相关领域的学术论文做铺垫。- ZJ
    
>[Coursera 课程](https://www.coursera.org/specializations/deep-learning) |
>[deeplearning.ai](https://www.deeplearning.ai/) |
>[网易云课堂](https://mooc.study.163.com/smartSpec/detail/1001319001.htm)

---
   转载请注明作者和出处：ZJ 
   
   深度学习知乎专栏：
   
   CSDN：
   
   [Github](https://github.com/laobadao/Deep-Learning)：https://github.com/laobadao/Deep-Learning
   
   简书：
   
   掘金：

---
## 1.1 Welcome

先来张 **Andrew Ng** 的帅图！


<img src="images/o-ANDREW-NG-facebook-1024x679.jpg" style="width:600px;height:400px;">

<font style='font-size:18px;line-height:1.75'>Hello and welcome,As you probably know, <font color=#0099ff>**Deep Learning**</font>  has aready transformed the traditional internet businesses,like web search and 
advertising.But deep learning is also enabling many new products and businesses in ways of helping people to recreate everything ranging from 
better healthcare, where deep learning is getting really good at reading X-ray images to the living personalize education to precision 
agriculture to even so driving cars and many others .</font><br /> 


<font style='font-size:15px;line-height:1.6'>大家好,欢迎各位,你们也许知道了,深度学习改变了传统互联网业务,例如如网络搜索和广告,但是深度学习同时也,使得许多新产品和企业,以很多方式帮助人们,从而获得更好的医疗保健。对此，深度学习做的非常好的一个方面就是,读取 X 光图像，再到生活中的个性化教育,到精准化农业,甚至到驾驶汽车,以及其它一些方面。</font><br /> 

<font style='font-size:18px;line-height:1.75'>If you want to learn the tools of deep learning and apply them to build these amazing things, I want to help you get there. When you finish this sequence courses on coursera call the specialization you'll be able to put deep learning on your resume with confidence.</font><br /> 

<font style='font-size:15px;line-height:1.6'>如果你想要学习深度学习的这些工具,并应用它们来做这些了不起的操作,我将帮助你做到这一点,当你完成 <font color=#0099ff>**coursera**</font> 上面的这一系列专项课程,你将能更加自信的继续深度学习之路。</font><br />

 <font style='font-size:18px;line-height:1.75'>Over the next decade I think all of us have the opportunity to build an amazing world and amazing society,that is AI's powers.I hope that you would play a big role in the creation of the AI society. So that, let's get started.I think that AI is the new electricity Started about 100 years ago,the electrification of our society transformed every major industry,everything ranging from transportation,manufacturing, healthcare,communications and many more.</font><br />

<img src="images/Supervising-AI-growth.jpg" style="width:600px;height:300px;">

<center>[Supervising AI Growth](https://futureoflife.org/2016/10/26/supervising-ai-growth/)</center>

- <font style='font-size:18px;line-height:1.75' color=#0099ff>AI is the new Electricity</font><br />
- <font style='font-size:18px;line-height:1.75'color=#0099ff>Electrification of our society transformed every major industry,everything ranging from transportation,manufacturing, healthcare,communications and many more</font><br />
- <font style='font-size:18px;line-height:1.75'color=#0099ff>AI now will to bring about an equally big transformation</font><br />



<font style='font-size:15px;line-height:1.6'>在接下来的十年中 我认为我们所有人都有机会创造一个惊人的世界和社会,这就是 AI（人工智能）的力量.我希望你们能发挥重要作用,在创建 AI（人工智能）社会的过程中,所以让我们开始吧,我认为 AI 是最新的电力,大约在一百年前,我们社会的电气化,改变了每个主要行业,从交通运输行业,到制造业、医疗保健、通讯等方面.</font><br />

 <font style='font-size:18px;line-height:1.75'>And I thinked today we see a surprisingly clear power of AI,to bring about an equally big transformation.And of course, the part of the AI that is rising rapidly driving along,with these developments is deep learning.So today, deep learning is one of the most highly sought-after skills in the technology world. And through this course and,a few courses after this one,I want to help you to gain,and master those skills.</font><br />

<font style='font-size:15px;line-height:1.6'>我认为如今我们见到了,AI 明显的令人惊讶的能量带来了同样巨大的转变,显然 AI 的各个分支中,发展的最为迅速的就是深度学习,因此现在深度学习是广受欢迎的,一种技巧,在科技世界中,通过这个课程,以及这门课程后门的几门课程,我想帮助你获取,并且掌握那些技能。</font><br />


## What you'll learn 


<font size='4'color=#0099f> **Courses in this sequence (specialization)**</font><br />

<font size='4'color=#0099f> 1. Neural Network and Deep Learning</font><br />
<font size='4'color=#0099f> 2. Improving Deep Neural Networks: Hyperparameter tuning,Regularization and Optimization</font><br />
<font size='4'color=#0099f> 3. Struct your machine learning project</font><br />
<font size='4'color=#0099f> 4. Convolutional Neural Networks</font><br />
<font size='4'color=#0099f> 5. Nature Language Processing: Building sequence Models</font><br />



<img src="images/ai-smart-city-952.jpg" style="width:600px;height:300px;">

<center>[NVIDIA AI CONFERENCE ](https://www.nvidia.com/en-sg/ai-conference/)</center>



<font style='font-size:18px;line-height:1.75'>So here's what you'll learn,in this sequence of courses,aslo called specialization on coursera.In the first course,you'll learn the Foundations of Neural Networks,you'll learn the Neural Network and Deep Learning.This video that you are watching is a part of this first course,which lasts four weeks in total.And each of the five courses in the specialization will be about 2 to 4 weeks,most of them actually will short than four weeks.But in this first course,you'll learn how to build a <font color=#0099ff>**Neural Network**</font> ,including a deep neural network,and how to train them on data.</font><br />

<font style='font-size:16px;line-height:1.6'>下面是你将学习到的内容,在 coursera 的这一系列也叫做微专业。在第一门课中,你将学习神经网络的基础,你将学习神经网络和深度学习。你观看的这个视频是第一门课的一部分,这门课将持续四周,专项课程中的每门课将持续 2 至 4 周,大部分将少于四周,但是在第一门课程中,您将学习如何建立神经网络,包含一个深度神经网络,以及如何在数据上面训练他们。</font><br />


<font style='font-size:18px;line-height:1.75'>And at the end of this course,you'll build a deep neural network to recognize and guess what? Cats.For some reason,there is a cat meme running around in deep learning.And so following tradition,this first course will build in cat recognize.Then, in the second course,you'll learn aobout the practical aspects of Deep Learning,you'll learn narrowly bulid neural network,how to actually get it perform well.So you'll learn about <font color=#0099ff>**hyperparameter tuning,regularization**</font> ,how to diagnose bias and variance,and advanced <font color=#0099ff>**optimization**</font> algorithms,like Momentum and Adam algorithm.</font><br />


<font style='font-size:16px;line-height:1.6'>在这门课程的结尾,你将用一个深度神经网络进行辨认,猜猜是什么？喵星人！由于某种原因,深度学习中会有一个猫的谜因运行。所以遵循传统,第一门课会以猫作为对象识别。接下来 在第二门课中,你将进行深度学习方面的实践,您将学习严密地构建神经网络,如何真正让它表现良好。因此你将要学习,超参数调整,正则化,诊断偏差和方差,以及一些高级优化算法,比如 Momentum 和 Adam 算法。</font><br />


<img src="images/cat.png" style="width:500px;height:600px;"><br />


<font style='font-size:18px;line-height:1.75'>Sometimes it seems like this allow the tuning ,even some black magic and how you build in your network.So the second course which is just three weeks will demystify so that black magic.In the third course, we'll just use two weeks,to learn how to struct your machine learning project.It turns out that the strategy for building a machine learning system has change the error of deep learning.So, for example,the way you split the data into train development or diff on most called validation set,and test sets has change the error of deep learnin.So what is the new best practice for doing that? And what of your train set and your test set come from different distributions,that's happening a lot more on the nueral deep learning.</font><br />

<font style='font-size:16px;line-height:1.6'>有时候看起来这样的调整是允许的，有如黑魔法一样根据你建立网络的方式，所以第二门课只有三周，来揭开这一黑魔法的神秘面纱，在第三门课中，我们将使用两周时间来学习如何结构化你的机器学习工程。事实证明，构建机器学习系统的策略，改变了深度学习的错误。举个例子，你分割数据的方式，分割成训练集 比较集或改变的验证集，以及测试集合，改变了深度学习的错误,所以最好的实践方式是什么呢？以及你的训练集和测试集,来自不同的贡献度在深度学习中的影响很大。</font><br />

<font style='font-size:18px;line-height:1.75'>So how do you deal that? And if you've heard of end-to-end deep learning,you'll also learn more about that in this third course,and see what you should use it,and maybe you shouldn't.The material in this third course is relatively unique.I'm going to share with you all of the hot-one lessons we have learnt,build and shaping quite of deeping learning problems,because I know ,is not taught in most common universities that have deep learning courses.But I think it really help you to get the deep learning system to work well.</font><br />

<font style='font-size:16px;line-height:1.6'>那么你应该怎么处理呢？如果你听说过端对端深度学习，你也会在第三门课中了解到更多，进而了解到你是否需要使用它，第三课的材料，是相对比较独特的，我将和你分享，我们了解到的所有的热门领域的，建立并且改良许多的深度学习问题，因为我知道，这是当今热门的材料在绝大部分大学里面不会教授的
，在他们的深度学习课堂上面，但我认为它会提供你帮助，让深度学习系统工作的更好。</font><br />

<font style='font-size:18px;line-height:1.75'>In the next course,we'll  then talk about Convolutional Neural Networks,ofen abbreviat to CNN(s).Convolutional Networks or,Convolutional Neural Networks,are often apply to images.So you'll learn how to build this model in course 4.</font><br />

<font style='font-size:16px;line-height:1.6'>在下一们课程中，我们将会提到，卷积神经网络，经常缩写为 CNN（s），卷积网络或者说卷积神经网络，经常被用于图像领域，所以你将会在第4门课程中学到如何搭建这样的模型。</font><br />

<font style='font-size:18px;line-height:1.75'>Finally in course 5,you'll learn sequence models,you'll learn sequence models,and how to apply them to  <font color=#0099ff>**nature language processing**</font>  and other problems.So sequence model include models like,<font color=#0099ff>**Recurrent Neural Network **</font> abbreviat to RNN,and <font color=#0099ff>**LSTM models stands for Long Short-Term Memory models **</font>,you'll learn what this term means in course 5,and be able to apply them to NLP problems,So you'll learn these models in course 5,and be able to apply them to sequence data,so for example, nature language is just a sequence of words,and you'll understand how this models can be apply to speech recognization or to music generation and other problems.</font><br />

<font style='font-size:16px;line-height:1.6'>最后在第5门课中，你将会学习到序列模型,以及如何将它们应用于自然语言处理,以及其它问题,序列模型包括的模型有,循环神经网络 简写为RNN,以及LSTM模型,全称是长短期记忆网络,你将在课程5中了解其中的时期是什么含义,并且有能力应用到NLP（自然语言处理）问题,总之你将在课程5中学习这些模型,以及能够将它们应用于序列数据,比如说 自然语言就是,一个单词序列,你也将能够理解这些模型如何应用到,语音识别,或者是编曲,以及其它问题。</font><br />

<font style='font-size:18px;line-height:1.75'>So through these courses,you'll learn the tools of deep learning,you'll be able to apply them,to bulid amazing things,And I hope many of you through this will also be able to advance your career.So that,let's get started,please go to the next video,we'll talk about deep learning,aplly to supervised learning.</font><br />

<font style='font-size:16px;line-height:1.6'>因此 通过这些课程,你将学习深度学习的这些工具,你将能够去使用它们,去做一些神奇的事情,我希望你们中的一些人,借此来提升你的职业生涯,因此,让我们一起开始,请进入下一个视频,我们将谈到深度学习在监督学习的使用。</font><br />


**PS: 欢迎扫码关注公众号：「SelfImprovementLab」！专注「深度学习」，「机器学习」，「人工智能」共同早起，学习，进步。** 


<img src="images/qrcode_for_gh_5f849a3079b0_344.jpg">

