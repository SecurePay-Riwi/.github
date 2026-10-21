<div align="center">

<img src="./securepay-logo.png" alt="SecurePay" width="180" />

# SecurePay

**Real-time anti-fraud, transaction monitoring and reconciliation for a digital wallet, built on AWS.**

[![Docs](https://img.shields.io/badge/docs-securepay--riwi.github.io-1f6feb?style=flat-square)](https://securepay-riwi.github.io/SecurePay/)
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-us--east--2-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)

</div>

---

## About

SecurePay builds **PagoSeguro Anti-fraud**, the platform that decides in under 200 ms whether each transaction of the PagoSeguro digital wallet is **approved**, **held for review** or **rejected**, and that reconciles the wallet with its payment partners every day.

- **Fast path:** a decision engine that answers from an in-memory cache, with velocity, mule account, transaction splitting, shared device, account takeover and restricted list rules.
- **Slow path:** every decision is published to SNS + SQS, where independent consumers open cases for analysts, keep device history and feed a three-layer Data Lake.
- **Built to run 24/7:** two Availability Zones, managed services first, and the cheapest option that does not give up security, availability or reliability.

## Repositories

| Repository | What it does |
| :--- | :--- |
| [**SecurePay**](https://github.com/SecurePay-Riwi/SecurePay) | The product: decision engine, consumers, local infrastructure and the documentation site |
| [**securepay-generator**](https://github.com/SecurePay-Riwi/securepay-generator) | Simulated transaction stream that plays the wallet's core, with labeled fraud patterns |
| [**securepay-apis**](https://github.com/SecurePay-Riwi/securepay-apis) | Daily exchange rates and a simulated restricted-list (PEP / sanctions) provider |
| [**securepay-csv**](https://github.com/SecurePay-Riwi/securepay-csv) | Kaggle datasets (PaySim, Sparkov) and the partners' daily statements |
| [**securepay-seed**](https://github.com/SecurePay-Riwi/securepay-seed) | Reproducible PostgreSQL seed and Kaggle ETL |

Shared models and config are published on PyPI as [`securepay-shared`](https://pypi.org/project/securepay-shared/).

## Tech stack

| Area | Technologies |
| :--- | :--- |
| Services | Python 3.12 · uv · FastAPI |
| Data | PostgreSQL · Valkey · DynamoDB · S3 Data Lake |
| Messaging | Amazon SNS + SQS with dead-letter queues |
| Compute | ECS Fargate · Lambda · Step Functions · EMR Serverless (PySpark) |
| Infrastructure | Terraform · GitHub Actions · Docker Compose + LocalStack for local work |
| Analytics | Glue · Athena · Power BI |

## Get started

Clone the repositories side by side and follow the [local setup guide](https://securepay-riwi.github.io/SecurePay/docs/getting-started/local-setup). To see the whole flow working on your machine, go to [Simulate the full flow](https://securepay-riwi.github.io/SecurePay/docs/getting-started/simulate-full-flow).

## Team

<table>
  <tr>
    <td align="center" width="160">
      <a href="https://github.com/inghabith"><img src="https://github.com/inghabith.png?size=200" width="96" alt="Habith" /><br /><b>Habith</b></a><br />
      <sub>Scrum Master / Team lead</sub>
    </td>
    <td align="center" width="160">
      <a href="https://github.com/Anndelgado"><img src="https://github.com/Anndelgado.png?size=200" width="96" alt="Yulianis" /><br /><b>Yulianis</b></a><br />
      <sub>Developer</sub>
    </td>
    <td align="center" width="160">
      <a href="https://github.com/Envy528"><img src="https://github.com/Envy528.png?size=200" width="96" alt="Jorge" /><br /><b>Jorge</b></a><br />
      <sub>Developer</sub>
    </td>
  </tr>
</table>

---

<div align="center">
<sub>Academic project at Riwi (Colombia). PagoSeguro is a fictional wallet and every piece of data in these repositories is synthetic or comes from public datasets.</sub>
</div>
