# commitcert-validation-workflows

Workflow **oficial** da plataforma CommitCert (reusable workflow).

O `ci.yml` de cada curso (no repo do aluno) apenas **chama** o
`.github/workflows/validate.yml` daqui. Como este repositório é seu e é
referenciado **fixado por um commit (SHA)**, o aluno não consegue adulterar o
que de fato roda — é a âncora de confiança do OIDC (`job_workflow_ref`).

> Mantenha este repo **público** e referencie-o sempre por SHA, nunca por branch,
> em produção (ver RFC §7 e Spike §7).
