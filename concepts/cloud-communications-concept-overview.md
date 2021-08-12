---
title: Обзор API облачных коммуникаций
description: API облачных коммуникаций в Microsoft Graph новое измерение взаимодействия приложений и служб с пользователями с помощью различных функций, связанных с коммуникацией, таких как вызовы и собрания в Интернете.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 81f7caf23c6e1ced7e98f5a907d073fa3bf18c66d725fe5b8376dcbd2c67e5c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246547"
---
# <a name="cloud-communications-api-overview"></a>Обзор API облачных коммуникаций
API облачных коммуникаций в Microsoft Graph новое измерение взаимодействия приложений и служб с пользователями с помощью различных функций, связанных с коммуникацией, таких как вызовы и собрания в Интернете. Развитие бизнеса путем ускорения реагирования на потребности клиентов и взаимодействия сотрудников друг с другом.

## <a name="why-integrate-with-the-cloud-communications-apis"></a>Зачем интегрироваться с API облачной связи?

Узнайте о преимуществах использования API облачных коммуникаций для создания приложений-служб[(ботов).](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)

### <a name="handle-incoming-calls"></a>Обработка входящих вызовов

Это может быть подавляющим время от времени, когда рабочие получают много бизнес-звонков, и это не возможно, или продуктивно, чтобы ответить на все из них. Бот может выполнять функции помощника на стойке регистрации и обрабатывать эти вызовы, отклоняя вызовы, которые кажутся нежелательными, и перенаправляя (переадресовыв) конкретные вызовы на другой номер.

API облачных коммуникаций можно использовать для:

- Чтобы пользователь позвонил [боту через](/graph/api/application-post-calls?view=graph-rest-1.0) VoIP.
- При необходимости [](/graph/api/call-redirect?view=graph-rest-1.0) бот перенаправляет входящий вызов соответствующему агенту.
- У бота [ответ](/graph/api/call-answer?view=graph-rest-1.0) или [отклонить](/graph/api/call-reject?view=graph-rest-1.0) вызов.


### <a name="simplify-the-customer-service-experience"></a>Упрощение работы с клиентами
Независимо от того, являетесь ли вы владельцем большой службы поддержки или небольшой витрины магазинов, может быть сложно обрабатывать несколько запросов клиентов, особенно если у вас нет контекста того, какую проблему они пытаются решить заранее. Обработка входящих вызовов от клиентов с помощью системы **интерактивного** голосового ответа (IVR), в которой бот изначально будет взаимодействовать с ними.

Если клиенту будет предложен ответ от бота, он может нажать клавишу на клавиатуре, соответствующую его выбору. После этого бот может собирать многочастотную частоту (DTMF) у клиента.

API облачных коммуникаций можно использовать для создания бота, который:

- [Отвечает на вызов](/graph/api/call-answer?view=graph-rest-1.0) клиента.
- [Воспроизведение запроса](/graph/api/call-playprompt?view=graph-rest-1.0) для информирования и запроса клиента для выбора.
- [Подписывается на тон,](/graph/api/call-subscribetotone?view=graph-rest-1.0) чтобы собрать DTMF от клиента.
- [Перевод клиента](/graph/api/call-transfer?view=graph-rest-1.0) агенту.
- [Завершает вызов](/graph/api/call-delete?view=graph-rest-1.0) с клиентом.

![Изображение бота, предоставляющий параметры для передачи вызовов](images/communications-ivr-transfer.png)

Чтобы создать более интеллектуальное взаимодействие между клиентами и ботом, когда клиенту будет предложен ответ, они смогут напрямую говорить о том, в чем им нужна помощь.

Интеграция со службой обработки естественного языка означает, что речь клиента может быть проанализирована для его настроений. Затем бот может соответствующим образом реагировать на потребности клиента.

>**Примечание:** Вы не можете записывать или иным образом сохранять медиаконтент из звонков или собраний, к которые ваше приложение имеет доступ, или данных, полученных из этого медиаконтента. Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений. Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

API облачных коммуникаций можно использовать для создания бота, который:

- [Отвечает на вызов](/graph/api/call-answer?view=graph-rest-1.0) клиента.
- [Воспроизводит подсказку,](/graph/api/call-playprompt?view=graph-rest-1.0) чтобы сообщить и побудить клиента к разговору.
- [Записывая короткий аудиозапись](/graph/api/call-record?view=graph-rest-1.0) выступления клиента.
- [Воспроизводит запрос](/graph/api/call-playprompt?view=graph-rest-1.0) с соответствующим ответом клиенту после анализа его речи.

![Изображение бота, который побуждает пользователя дать голосовой ответ](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a>Совместное взаимодействие с помощью групповых вызовов
Включить пользователей для общения с коллегами или клиентами, создав групповой вызов, чтобы каждый может внести свой вклад в беседу.

API облачных коммуникаций можно использовать для создания бота, который:

- [Создает групповой вызов с](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) несколькими участниками.
- [Приглашает другого бота или пользователя к](/graph/api/participant-invite?view=graph-rest-1.0) существующему групповому вызову.
- [Присоединяется к существующему групповому вызову](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) в качестве бота.
- [Списки участников](/graph/api/call-list-participants?view=graph-rest-1.0) группового вызова.
- [Приглушает другого участника.](/graph/api/participant-mute?view=graph-rest-1.0)

### <a name="send-reminders-reliably"></a>Отправка напоминаний надежно
Чтобы пользователи могли отправлять клиентам напоминание о встрече или напоминание о приближающихся сроках оплаты, вы можете автоматически вызвать клиента ботом. <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

API облачных коммуникаций можно использовать для создания бота, который:

- [Вызывает клиента на](/graph/api/application-post-calls?view=graph-rest-1.0) Teams.
- [Воспроизводит записанную подсказку,](/graph/api/call-playprompt?view=graph-rest-1.0) которая служит напоминанием.
- [Завершает вызов.](/graph/api/call-delete?view=graph-rest-1.0)


### <a name="set-up-online-meetings"></a>Организация собраний по сети
Планирование собрания между врачом и пациентом или между пользователем и его прямыми отчетами позволяет создавать решения, на которые можно положиться пользователям. Для большей гибкости пользователи могут вызывать других пользователей и приглашать их на собрание, пока оно продолжается.

API облачных коммуникаций можно использовать для:

- Чтобы пользователь [создал собрание в Интернете.](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)
- У пользователя [получить сведения о](/graph/api/onlinemeeting-get?view=graph-rest-1.0) собрании в Интернете.
- Чтобы бот или пользователь [присоединились к собранию в Интернете.](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API облачных коммуникаций в Microsoft Graph (v1.0)](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [API облачных коммуникаций в Microsoft Graph (бета-версия)](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Используйте боты, [чтобы начать работу.](cloud-communications-get-started.md)
- Дополнительные новости о [звонках,](cloud-communications-calls.md) [медиа и](cloud-communications-media.md) [собраниях в Интернете.](cloud-communications-online-meetings.md)
- Просмотр ограничений [использования](throttling.md#cloud-communication-service-limits)API.
- Узнайте, как [управлять номерами телефонов](cloud-communications-phone-number.md) для ботов.

## <a name="see-also"></a>См. также

- [Разрешения приложений и делегированные разрешения](/azure/active-directory/develop/v1-permissions-and-consent)
- [Разрешения звонков](./permissions-reference.md#calls-permissions)
- [Разрешения на собрания в Интернете](./permissions-reference.md#online-meetings-permissions)
- [Примеры облачных коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
