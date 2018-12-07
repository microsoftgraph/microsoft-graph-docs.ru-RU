---
title: Использование API безопасности Microsoft Graph
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: dff91665fc288bf1714d1975f3ec2e109f576530
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184534"
---
# <a name="use-the-microsoft-graph-security-api"></a>Использование API безопасности Microsoft Graph

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

API-Интерфейс безопасности Microsoft Graph предоставляет единый интерфейс и схемы можно интегрировать с решения по обеспечению безопасности корпорации Майкрософт и экосистема партнеров. Это позволяет предоставить клиентам для оптимизации операции по безопасности и более надежную защиту от увеличение угрозы, связанные с через Интернет. API Microsoft Graph безопасности можно использовать как службы объединение федеративных безопасности для отправки запросов для всех поставщиков безопасности onboarded для получения групп ответов. Использовать Microsoft Graph безопасности API для создания приложений, который:

- Объединение и их оповещение системы безопасности из нескольких источников
- Разблокировать контекстных данных для оповещения исследования
- Операции по безопасности для повышения эффективности автоматизации
- Обеспечивает возможность отслеживания данных безопасности для включения проактивное управление рисками

API-Интерфейс Microsoft Graph безопасности включает в себя следующие основные сущности.

## <a name="alerts"></a>Оповещения

Оповещения, потенциальных проблем безопасности в клиент пользователя, который решения по обеспечению безопасности Майкрософт или партнер идентификации и отмеченные на действие или уведомление. С помощью объекта [оповещений](alert.md) безопасности Microsoft Graph можно объединяют в себе и оптимизируют проблемы безопасности через все интегрированные решения. Это также позволяет приложениям для корреляции оповещений и контекста для улучшения защиты от угроз и ответа. Эти разблокировать эффективность безопасности, сокращая время расследования и разрешения для обращения в службу. Возможность обновления оповещений можно синхронизировать состояние определенных предупреждений по безопасности продуктов и служб, интегрированных с Microsoft Graph безопасности API, изменив сущности [оповещения](alert.md) .

Интегрированное графическое представление безопасности решения Майкрософт будет получать оповещения от следующих поставщиков безопасности:

- [Центр безопасности для Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Безопасность приложений Microsoft Cloud](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Защитник Windows Advanced защиту от угроз](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Защита информации Azure](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(Предварительная версия)**
- Microsoft Intune **(закрытый Предварительная версия)**
- Office 365 **(ожидается в ближайшее время)**
- Azure расширенного защиту от угроз **(ожидается в ближайшее время)**
- Решений партнеров, такими как компьютер Пало сетей приложения Framework

> **Примечание:** Новые поставщики постоянно, входящая экосистемы Microsoft Graph безопасности.

## <a name="secure-score-preview"></a>Secure показатель (Предварительная версия)

[Оценки безопасности Microsoft](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) — это решение analytics безопасности, задающей видимости в Портфель безопасности и способы повышения его. С одним индексом лучше понять Готово для снижения риска в решения Майкрософт. Можно также сравнение результатов с другими организациями и увидеть, как прибора результатов по времени. Microsoft Graph безопасности [secureScore](securescores.md) и [secureScoreControlProfiles](securescorecontrolprofiles.md) сущности, посвященные сбалансировать потребности вашей организации безопасность и производительность при включении соответствующего разные возможности обеспечения безопасности. Можно также project результатов, которые может быть после внедрять функции обеспечения безопасности.

## <a name="common-use-cases"></a>Основные сценарии выполнения

Ниже приведены некоторые из наиболее популярные запросы для работы с Microsoft Graph безопасности API.

| **Варианты использования**   | **Ресурсы REST** | **Попробуйте прямо в обозревателе график** |
|:---------------|:--------|:----------|
| перечисление оповещений; | [перечисление оповещений](../api/alert-list.md); | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [обновление оповещения](../api/alert-update.md). | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Список безопасных показателям|[Список secureScores](../api/securescores-list.md) (Предварительная версия)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Список безопасного элемента управления профилями показатель|[Список secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (Предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Обновление безопасного элемента управления профилями показатель|[Обновление secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (Предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Можно использовать Microsoft Graph [webhooks](/graph/webhooks) подписаться на и получать уведомления об обновлениях для сущности Microsoft Graph безопасности.

## <a name="next-steps"></a>Дальнейшие действия

API-Интерфейс безопасности Microsoft Graph может привести к возникновению новые способы работы с решениями безопасности, отличные от корпорации Майкрософт и партнеров. Выполните следующие действия, чтобы приступить к работе.

- Перейти к [оповещения](alert.md), [secureScore](securescores.md) (Предварительная версия) и [secureScoreControlProfiles](securescorecontrolprofiles.md) (Просмотр).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). В разделе **Примеры запросов**выберите команду **Показать дополнительные примеры** и установите категории безопасности **на**.
- Попробуйте [подпиской и получение уведомлений](/graph/webhooks) на изменения сущности.

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>См. также

Примеры кода и внесение данных в этих примерах Microsoft Graph безопасности API:

- [Пример ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример с Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Начните работать с сообществом:

- [Присоединяйтесь к сообществу Технический](https://aka.ms/graphsecuritycommunity)
- [Обсудить на StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
