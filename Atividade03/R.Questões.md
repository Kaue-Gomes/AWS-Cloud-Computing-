1. Qual a diferença entre armazenamento de objetos (S3) e armazenamento em bloco (EBS)?

O Amazon S3 (Simple Storage Service) utiliza armazenamento de objetos, onde os arquivos são armazenados como objetos contendo dados, metadados e um identificador único. Ele é ideal para armazenar documentos, imagens, vídeos, backups e arquivos em geral, oferecendo alta escalabilidade e durabilidade.

Já o Amazon EBS (Elastic Block Store) utiliza armazenamento em bloco, funcionando como um disco rígido virtual conectado a uma instância EC2. Os dados são divididos em blocos e podem ser utilizados por sistemas operacionais e bancos de dados que necessitam de acesso rápido e frequente aos dados.

2. Por que o nome do bucket precisa ser único no mundo inteiro?

O nome de um bucket S3 precisa ser globalmente único porque todos os buckets da AWS compartilham um espaço de nomes global. Isso permite que cada bucket seja identificado de forma exclusiva por meio de URLs e APIs.

3. O link temporário que você gerou vai funcionar para sempre? Por quê?

Não. O Presigned URL possui uma data e hora de expiração definidas no momento da sua criação.

Após o prazo configurado (por exemplo, 1 hora, 12 horas ou 7 dias), o link deixa de funcionar automaticamente porque a assinatura de segurança embutida na URL expira.

Isso aumenta a segurança, permitindo compartilhar arquivos temporariamente sem torná-los públicos permanentemente.