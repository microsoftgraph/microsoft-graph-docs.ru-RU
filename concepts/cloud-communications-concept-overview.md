---
title: Общие сведения об API облачных коммуникаций
description: API облачных коммуникаций в Microsoft Graph добавляют новое измерение, в соответствии с которыми ваши приложения и службы взаимодействуют с пользователями с помощью различных компонентов, связанных с взаимодействием, таких как звонки и собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: fc8ab5e91ba16a2b9dc0730120be350550caf145
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050780"
---
# <a name="cloud-communications-api-overview"></a>Общие сведения об API облачных коммуникаций
API облачных коммуникаций в Microsoft Graph добавляют новое измерение, в соответствии с которыми ваши приложения и службы взаимодействуют с пользователями с помощью различных компонентов, связанных с взаимодействием, таких как звонки и собрания по сети. Развивайте свой бизнес, отменяя способы реагирования на потребности клиентов и взаимодействие сотрудников друг с другом.

## <a name="why-integrate-with-the-cloud-communications-apis"></a>Зачем выполнять интеграцию с API облачных коммуникаций?

Узнайте о преимуществах использования API облачных коммуникаций для приложений-служб Буид ([Боты](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)).

### <a name="handle-incoming-calls"></a>Обработка входящих вызовов

Это может быть затруднительно, когда работники получают большое количество бизнес-звонков, а также не могут (или продуктивно) отвечать на них. С помощью ленты, созданной в качестве помощника по обслуживанию переднего плана, можно отклонить, что кажется нежелательным, и перенаправлением (перенаправлением) определенных вызовов на другой номер.

API облачных коммуникаций можно использовать для следующих действий:

- Пользователь [звонит](/graph/api/application-post-calls?view=graph-rest-1.0) через VoIP через VoIP.
- При необходимости [перенаправьте входящий вызов](/graph/api/call-redirect?view=graph-rest-1.0) соответствующему агенту.
- Попросите [или](/graph/api/call-answer?view=graph-rest-1.0) [отклонить](/graph/api/call-reject?view=graph-rest-1.0) вызов.


### <a name="simplify-the-customer-service-experience"></a>Упрощение взаимодействия со службой клиентов
Независимо от того, кто владеет большой службой технической поддержки или небольшим витриной, может быть трудно обрабатывать несколько запросов клиентов, особенно если у вас нет контекста проблемы, с которой они попытаются решить заранее. Обработка входящих вызовов от клиентов через систему **интерактивного речевого ответа** (IVR), которая изначально будет взаимодействовать с ними.

Когда клиент запрашивает ответ от Bot, клиент может нажать клавишу на клавиатуре, соответствующей выделенному фрагменту. Затем он может собрать многочастотный набор (DTMF) с клиента.

Вы можете использовать API Cloud Communications для создания объекта Bot, который:

- [Отвечает на вызов](/graph/api/call-answer?view=graph-rest-1.0) от клиента.
- [Воспроизводит запрос](/graph/api/call-playprompt?view=graph-rest-1.0) для уведомления и приглашения клиента на выбор.
- [Подписывается на тон](/graph/api/call-subscribetotone?view=graph-rest-1.0) , чтобы получить информацию о DTMF от клиента.
- [Передает клиента](/graph/api/call-transfer?view=graph-rest-1.0) агенту.
- [Завершает вызов](/graph/api/call-delete?view=graph-rest-1.0) с клиентом.

![Изображение объекта Bot, предоставляющего параметры для передачи вызовов](images/communications-ivr-transfer.png)

Чтобы создать более интеллектуальное взаимодействие между клиентами и Bot, когда клиент запрашивает ответ, он сможет напрямую говорить о том, что им нужна помощь.

Интеграция со службой "естественная языковая обработка" означает, что голосовая речь пользователя может быть проанализирована для его мнений. Затем Bot может отвечать на запросы клиента соответствующим образом.

>**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента. Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций. Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

Вы можете использовать API Cloud Communications для создания объекта Bot, который:

- [Отвечает на вызов](/graph/api/call-answer?view=graph-rest-1.0) от клиента.
- [Воспроизводит запрос](/graph/api/call-playprompt?view=graph-rest-1.0) для информирования клиента о том, что он говорите.
- [Запись короткого](/graph/api/call-record?view=graph-rest-1.0) аудиоклипа клиента.
- [Воспроизводит приглашение](/graph/api/call-playprompt?view=graph-rest-1.0) с соответствующим ответом клиенту после анализа речи.

![Изображение элемента Bot, с помощью которого пользователь получает голосовый ответ](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a>Сотрудничество через групповые звонки
Разрешите пользователям привлекать сотрудников или клиентов, создавая групповой звонок, чтобы все могли участвовать в беседе.

Вы можете использовать API Cloud Communications для создания объекта Bot, который:

- [Создает групповой вызов](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) с несколькими участниками.
- [Приглашает другого пользователя или пользователя](/graph/api/participant-invite?view=graph-rest-1.0) к существующему групповому вызову.
- [Присоединяется к существующему групповому вызову](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) в качестве Bot.
- [Выводит список участников](/graph/api/call-list-participants?view=graph-rest-1.0) группового звонка.
- [Отключение выключения другого участника](/graph/api/participant-mute?view=graph-rest-1.0).

### <a name="send-reminders-reliably"></a>Надежная Отправка напоминаний
Чтобы пользователи могли отправлять клиенту напоминание о встрече или напоминании о приближающемся сроке платежа, можно автоматически позвонить клиенту. <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

Вы можете использовать API Cloud Communications для создания объекта Bot, который:

- [Вызывает клиента](/graph/api/application-post-calls?view=graph-rest-1.0) в Teams.
- [Воспроизводит записанный запрос](/graph/api/call-playprompt?view=graph-rest-1.0) , который служит напоминанием.
- [Завершает вызов](/graph/api/call-delete?view=graph-rest-1.0).


### <a name="set-up-online-meetings"></a>Настройка собраний по сети
При планировании собрания между врачом и пациентом, а также между пользователем и их прямыми отчетами можно создавать решения, которые создают собрания, на которых могут полагаться пользователи. Для повышения гибкости пользователи могут звонить другим пользователям и присоединиться к собранию во время их выполнения.

API облачных коммуникаций можно использовать для следующих действий:

- Попросите пользователя [создать собрание по сети](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0).
- Пользователь [получает сведения о](/graph/api/onlinemeeting-get?view=graph-rest-1.0) собрании по сети.
- [Присоединитесь к собранию по сети](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)с помощью Bot или пользователя.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API облачных коммуникаций в Microsoft Graph (версия 1.0)](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [API облачных коммуникаций в Microsoft Graph (бета-версия)](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Чтобы приступить к [работе](cloud-communications-get-started.md), используйте Боты.
- Узнайте больше о [звонках](cloud-communications-calls.md), [мультимедиа](cloud-communications-media.md)и [собраниях по сети](cloud-communications-online-meetings.md).
- Просмотр [пределов](throttling.md#cloud-communication-service-limits)использования API.
- Узнайте, как [управлять номерами телефонов](cloud-communications-phone-number.md) для вашего Боты.

## <a name="see-also"></a>См. также

- [Делегированные разрешения и разрешения для приложений](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent)
- [Разрешения звонков](/graph/permissions-reference#calls-permissions)
- [Разрешения для собраний по сети](/graph/permissions-reference#online-meetings-permissions)
- [Примеры облачных коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples)


