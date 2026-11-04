# TinyBeauty — ROI de cores de maquiagem
Duas continuações controladas do mesmo BeautyREC48 de 20.000 passos: (1) supervisão por pixels alterados de lip/eyelid, (2) mesma supervisão mais direção/crominância da alteração. +500/+1500/+2500 passos. Checkpoints do mesmo teacher V4 plane_iris_pixels, mesmas 1000 imagens treino /136 validação e seed.
Todas as comparações são no mesmo grupo de 8 pessoas; para cada versão há output bruto e saída com máscara protetora. As métricas dos novos modelos são medidas depois da máscara e não devem ser usadas no modo bruto.
