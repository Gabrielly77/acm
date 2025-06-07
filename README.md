# acm

ACM na AWS é o AWS Certificate Manager.

Sabe quando tu precisa de certificado SSL/TLS pra deixar teu site ou app seguro, com aquele cadeadinho verde no navegador? Então, o ACM é o serviço que ajuda a criar, gerenciar e renovar esses certificados automaticamente, sem aquele perrengue manual de ficar gerando CSR, validando, instalando... tudo na mão.

Na prática, tu pede o certificado pro ACM, ele emite (às vezes com validação por email ou DNS), e depois tu pode usar esse certificado em vários serviços da AWS, tipo:

Elastic Load Balancer (ELB) - pra proteger a comunicação entre o usuário e teu app;

CloudFront - pra CDN segura;

API Gateway - pra proteger suas APIs;

e outros serviços que suportam TLS.

Isso facilita demais, porque é grátis, e a AWS cuida da renovação automática, evitando o problema clássico do certificado expirado e site fora do ar.
