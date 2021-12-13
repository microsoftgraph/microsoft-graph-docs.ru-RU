---
title: Обзор API отчетов для обучения симуляции атаки в рамках Microsoft Defender для Office 365
description: В этом разделе описываются API, обладающие доступом к отчетам безопасности, которые являются частью Microsoft Defender для Office 365.
ms.localizationpriority: high
author: Gopal-MSFT
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 76d41d429145da44d7d094d3a0d310a7e6a0c142
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424758"
---
# <a name="reports-api-overview-for-attack-simulation-training-as-part-of-microsoft-defender-for-office-365"></a>Обзор API отчетов для обучения симуляции атаки в рамках Microsoft Defender для Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В этом разделе описываются возможности создания отчетов Microsoft Defender для Office 365, в частности API, которые обладают доступом к отчетам об участии клиента в обучении симуляции атаки. Обучение симуляции атаки подготавливает неопасные имитации кибератак, чтобы обучать пользователей в клиенте с целью повышения их осведомленности и выявления уязвимых пользователей.

## <a name="what-role-do-the-attack-simulation-reports-play-in-enterprise-defense"></a>Какую роль отчеты о симуляции атак играют в защите предприятия?

Отчеты о симуляции атак помогают администраторам клиентов выявлять пробелы в знаниях о безопасности, чтобы они могли дополнительно обучать пользователей с целью снижения их восприимчивости к атакам. Служба обучения симуляции атаки является частью [Microsoft Defender для Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) и защищает вашу организацию от угроз, содержащихся в электронных письмах, ссылках (URL-адресах) и средствах совместной работы.

Microsoft Defender для Office 365 входит в набор [Microsoft 365 Defender](/microsoft-365/security/defender/microsoft-365-defender?view=o365-worldwide&preserve-view=true), который включает указанные ниже службы.

- [Microsoft Defender для конечной точки](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)
- [Microsoft Defender для Office 365](/microsoft-365/security/office-365-security/overview)
- [Microsoft Defender для удостоверений](/defender-for-identity/)
- [Microsoft Defender for Cloud Apps](/cloud-app-security/)

Microsoft 365 Defender — это единый набор корпоративной защиты для обнаружения рисков безопасности, исследования атак в организации и автоматического предотвращения вредоносных действий. Он предоставляет портал центрального администрирования ([https://security.microsoft.com/](https://security.microsoft.com)), объединяющий средства защиты, обнаружения, исследования и реагирования на угрозы _электронной почты_, _совместной работы_, _удостоверений_ и _устройств_.

Чтобы получить доступ к обучению симуляции атаки, откройте портал Microsoft 365 Defender и выберите **Сообщения электронной почты и совместная работа** > **Обучение симуляции атаки**.


## <a name="authorization"></a>Авторизация

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Укажите разрешения, необходимые для доступа к отчетам. Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для отчетов](/graph/permissions-reference#reports-permissions).

## <a name="what-kinds-of-data-do-the-reports-return"></a>Какие типы данных возвращают отчеты?

| Типы данных          | Ресурс                                | API         |
|:---------------------- |:--------------------------------------- |:------------|
| Уязвимые периодические нарушители в клиенте | [attackSimulationRepeatOffender](attacksimulationrepeatoffender.md) | [getAttackSimulationRepeatOffenders](../api/reportroot-getattacksimulationrepeatoffenders.md) |
| Данные и результаты симуляции для каждого пользователя в клиенте | [attackSimulationSimulationUserCoverage](attacksimulationsimulationusercoverage.md) | [getAttackSimulationSimulationUserCoverage](../api/reportroot-getattacksimulationsimulationusercoverage.md) |
| Пройденное обучение для каждого пользователя в клиенте | [attackSimulationTrainingUserCoverage](attacksimulationtrainingusercoverage.md) | [getAttackSimulationTrainingUserCoverage](../api/reportroot-getattacksimulationtrainingusercoverage.md) |

## <a name="next-steps"></a>Дальнейшие действия

Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

