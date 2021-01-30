---
title: Обзор API облачных коммуникаций
description: API облачных коммуникаций в Microsoft Graph добавляют новое измерение взаимодействия приложений и служб с пользователями с помощью различных функций, связанных с связью, таких как вызовы и собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 572ce19e14779615ac8db514101df7d944b1d819
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059597"
---
# <a name="cloud-communications-api-overview"></a>Обзор API облачных коммуникаций
API облачных коммуникаций в Microsoft Graph добавляют новое измерение взаимодействия приложений и служб с пользователями с помощью различных функций, связанных с связью, таких как вызовы и собрания по сети. Развивать свой бизнес, ускоряя реагирование на потребности клиентов и взаимодействие сотрудников друг с другом.

## <a name="why-integrate-with-the-cloud-communications-apis"></a>Зачем интегрироваться с API облачных коммуникаций?

Узнайте о преимуществах использования API облачных коммуникаций для создания приложений-служб[(ботов).](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)

### <a name="handle-incoming-calls"></a>Обработка входящих вызовов

Иногда, когда сотрудники получают большое количество бизнес-вызовов и невозможно или продуктивно ответить на все из них, это может ошеломить. Бот может выступать в качестве помощника службы поддержки и обрабатывать эти вызовы, отклоняя такие вызовы, как спам, и перенаправляя (перенаправляя) определенные вызовы на другой номер.

API облачных коммуникаций можно использовать для:

- Пользователь должен позвонить [боту через](/graph/api/application-post-calls?view=graph-rest-1.0) VoIP.
- При необходимости бот [перенаправляет](/graph/api/call-redirect?view=graph-rest-1.0) входящий вызов соответствующему агенту.
- Ответ [бота или](/graph/api/call-answer?view=graph-rest-1.0) [отклонение](/graph/api/call-reject?view=graph-rest-1.0) вызова.


### <a name="simplify-the-customer-service-experience"></a>Упрощение обслуживания клиентов
Независимо от того, являетесь ли вы владельцем большой службы поддержки или небольшого магазина, может быть трудно обрабатывать несколько запросов клиентов, особенно если у вас нет контекста проблемы, которые они пытаются решить заранее. Обработка входящих вызовов  от клиентов с помощью системы интерактивного голосового ответа (IVR), где бот изначально будет взаимодействовать с ними.

Когда клиенту будет предложено получить ответ от бота, он может нажать клавишу на клавиатуре, соответствующую его выбору. Затем бот может собрать многочастотный набор DTMF от клиента.

Вы можете использовать API облачных коммуникаций для создания бота, который:

- [Отвечает на звонок](/graph/api/call-answer?view=graph-rest-1.0) от клиента.
- [Воспроизводит подсказку](/graph/api/call-playprompt?view=graph-rest-1.0) для информирования и запроса выбора.
- [Подписка на тон для](/graph/api/call-subscribetotone?view=graph-rest-1.0) сбора DTMF от клиента.
- [Перевод клиента](/graph/api/call-transfer?view=graph-rest-1.0) агенту.
- [Завершает звонок](/graph/api/call-delete?view=graph-rest-1.0) с клиентом.

![Изображение бота, предоставляющий параметры для передачи вызовов](images/communications-ivr-transfer.png)

Чтобы создать более интеллектуальное взаимодействие между клиентами и ботом, когда клиенту будет предложен ответ, он сможет напрямую говорить о том, с чем им нужна помощь.

Интеграция со службой обработки естественного языка означает, что речь клиента можно проанализировать на его тональность. После этого бот сможет отвечать на запросы клиента соответствующим образом.

>**Примечание.** Вы не можете записывать или иным образом сохранять содержимое мультимедиа из звонков или собраний, к которые ваше приложение имеет доступ, или данные, полученные из этого содержимого мультимедиа. Убедитесь, что вы соответствуете законам и нормативным актам вашей области в отношении защиты данных и конфиденциальности коммуникаций. Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

Вы можете использовать API облачных коммуникаций для создания бота, который:

- [Отвечает на звонок](/graph/api/call-answer?view=graph-rest-1.0) от клиента.
- [Воспроизводит подсказку](/graph/api/call-playprompt?view=graph-rest-1.0) для информирования и запроса клиента на разговор.
- [Записи короткого звукового клипа,](/graph/api/call-record?view=graph-rest-1.0) в который говорит клиент.
- [Воспроизводит подсказку](/graph/api/call-playprompt?view=graph-rest-1.0) с соответствующим ответом клиенту после анализа его речи.

![Изображение бота, который дает пользователю запрос на голосовой ответ](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a>Совместное взаимодействие с помощью групповых звонков
Позволяет пользователям взаимодействовать с коллегами или клиентами, создавая групповой звонок, чтобы все могли участвовать в беседе.

Вы можете использовать API облачных коммуникаций для создания бота, который:

- [Создает групповой звонок с](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) несколькими участниками.
- [Приглашает другого бота или пользователя к](/graph/api/participant-invite?view=graph-rest-1.0) существующему групповому вызову.
- [Присоединяется к существующему групповому вызову](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) в качестве бота.
- [Перечисляет участников](/graph/api/call-list-participants?view=graph-rest-1.0) группового вызова.
- [Отключает другого участника.](/graph/api/participant-mute?view=graph-rest-1.0)

### <a name="send-reminders-reliably"></a>Надежно отправлять напоминания
Чтобы пользователи могли отправлять клиентам напоминания о встрече или напоминания о приближении крайнего срока оплаты, вы можете вызвать клиента автоматически. <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

Вы можете использовать API облачных коммуникаций для создания бота, который:

- [Звонит клиенту в](/graph/api/application-post-calls?view=graph-rest-1.0) Teams.
- [Воспроизводит записанную подсказку](/graph/api/call-playprompt?view=graph-rest-1.0) в качестве напоминания.
- [Завершает вызов.](/graph/api/call-delete?view=graph-rest-1.0)


### <a name="set-up-online-meetings"></a>Организация собраний по сети
Независимо от того, запланируйте ли вы собрание между пациентов и пациентов или между пользователем и их прямыми отчетами, вы можете создавать решения, которые создают собрания, на которые могут полагаться пользователи. Для большей гибкости пользователи могут звонить другим пользователям и приглашать их на собрание во время его проведения.

API облачных коммуникаций можно использовать для:

- Пользователь должен [создать собрание по сети.](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)
- Пользователь должен [получить сведения о](/graph/api/onlinemeeting-get?view=graph-rest-1.0) собрании по сети.
- Бот или пользователь должны присоединиться [к собранию по сети.](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API облачных коммуникаций в Microsoft Graph (1.0)](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [API облачных коммуникаций в Microsoft Graph (бета-версия)](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Использование ботов для [начала работы.](cloud-communications-get-started.md)
- Узнайте больше о [звонках,](cloud-communications-calls.md) [мультимедиа](cloud-communications-media.md)и [собраниях по сети.](cloud-communications-online-meetings.md)
- Просмотр ограничений [использования](throttling.md#cloud-communication-service-limits)API.
- Узнайте, как [управлять номерами телефонов](cloud-communications-phone-number.md) для ботов.

## <a name="see-also"></a>См. также

- [Делегирование разрешений и разрешений приложений](/azure/active-directory/develop/v1-permissions-and-consent)
- [Разрешения звонков](./permissions-reference.md#calls-permissions)
- [Разрешения собраний по сети](./permissions-reference.md#online-meetings-permissions)
- [Примеры облачных коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
