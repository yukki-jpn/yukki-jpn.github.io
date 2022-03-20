# Reduced Order Book Dynamics
<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>
ここでは、LOBダイナミクスを理解するために、まずLOBを構成する各Queue (1st, 2nd, 3rd...) を数理モデル化しよう。

![LOB](FirstQueueDynamics.png)

## Independent Queue Dynamics: Fokker-Planck Approach
ここでは、LOBのダイナミクスに関して、リアルタイムで観測可能な**Queueの増減**とヒストリカルデータで観測可能な**指値・成行・キャンセル注文**に分けてモデル化を行おう。

### Queue Dynamics
Assumption: Markov dynamics