---
title: Получение общего или делегированного календаря Outlook и его событий
description: В Outlook владелец календаря может поделиться им с другими пользователями и предоставить им доступ на просмотр или изменение событий в своем календаре. Календарь может быть пользовательским или основным. Владелец также может предоставить делегату право выполнять действия от его имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в основном календаре учетной записи электронной почты.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 06e11f11b9c25e3392075e027278558d1330d51e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470076"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a>Получение общего или делегированного календаря Outlook и его событий

В Outlook владелец календаря может поделиться им с другими пользователями и предоставить им доступ на просмотр или изменение событий в своем календаре. Общий календарь может быть основным календарем владельца или пользовательским календарем, созданным владельцем. Владелец также может предоставить делегату для своего основного календаря право выполнять действия от его имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в основном календаре.

Что касается программного кода, Microsoft Graph поддерживает чтение и запись событий в календарях, доступ к которым был предоставлен другими пользователями, а также чтение общих календарей и обновление их имен для получателей общего доступа. Поддержка также относится к делегированным календарям. Далее в этой статье описывается чтение событий в общем или делегированном календаре. Сведения о создании событий см. в статье [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md).

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a>Получатель общего доступа: получение общего календаря или его событий непосредственно из почтового ящика владельца календаря

В трех примерах, приведенных ниже, используется следующий сценарий: Артем поделился своим основным календарем с Мартой в Outlook и предоставил ей разрешения на чтение. Если Марта войдет в приложение и предоставит _делегированные разрешения_ (Calendars.Read.Shared или Calendars.ReadWrite.Shared) от своего имени, приложение сможет получить доступ к основному календарю Артема и его событиям непосредственно из почтового ящика Артема.

В трех примерах указан идентификатор владельца (ИД пользователя или имя участника-пользователя Артема) и ярлык `calendar`. У них есть доступ к идентификаторам календаря и событий, которые соответствуют почтовому ящику владельца. При указании идентификаторов календаря и событий в почтовом ящике получателя общего доступа (идентификатор пользователя или имя участника-пользователя Марты) будет возвращена ошибка. Сведения об использовании идентификаторов календаря и событий, которые соответствуют почтовому ящику получателя общего доступа, см. в разделе [Получатель общего доступа: получение общего пользовательского календаря или его событий из почтового ящика получателя общего доступа](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox). 

> **Примечание.** Разрешения общего доступа (Calendars.Read.Shared или Calendars.ReadWrite.Shared) позволяют читать или записывать события в общем или делегированном календаре. Они не поддерживают [подписку на уведомления об изменениях](webhooks.md) элементов в таких папках. Чтобы настроить подписки на уведомления об изменениях событий в общем, делегированном или любом другом календаре пользователя или ресурса в клиенте, используйте разрешение приложения Calendars.Read.

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Марта: получение общего основного календаря непосредственно из почтового ящика Артема

Войдя в систему под именем Марты, получите основной календарь, которым Артем поделился с Мартой, непосредственно из почтового ящика Артема.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [calendar](/graph/api/resources/calendar?view=graph-rest-1.0), представляющий общий основной календарь Артема, в его почтовом ящике.

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Марта: получение события общего основного календаря непосредственно из почтового ящика Артема

При выполнении входа в систему под именем Марты приложение может получить определенное событие основного календаря, которым Артем поделился с Мартой, непосредственно из его почтового ящика.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [event](/graph/api/resources/event?view=graph-rest-1.0), определенный параметром `{id}` в основном календаре Артема, непосредственно из его почтового ящика.

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a>Марта: получение всех событий общего основного календаря из почтового ящика Артема

Войдя в систему под именем Марты, получите все события основного календаря, которым Артем поделился с Мартой, непосредственно из его почтового ящика.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [event](/graph/api/resources/event?view=graph-rest-1.0) в основном календаре Артема непосредственно из его почтового ящика.

Те же возможности GET доступны в том случае, если Артем делегировал Марте доступ к своему основному календарю или если Артем делегировал Марте весь свой почтовый ящик.

Если Артем не предоставил общий доступ к своему основному календарю и не делегировал его Марте, при указании ИД пользователя или имени участника-пользователя Артема будет возвращена ошибка. 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a>Получатель общего доступа: получение общего пользовательского календаря или его событий из почтового ящика получателя общего доступа

Если Артем поделился _пользовательским_ календарем (например, календарем «Детские праздники») с Анной и Анна предоставила делегированные разрешения (Calendars.Read или Calendars.ReadWrite), приложение может получить события или календарь из локальной копии календаря Артема в почтовом ящике Анны, как описано ниже.

1. Войдя в систему под именем Анны, используйте один из следующих запросов, чтобы получить все календари, к которым Анна имеет доступ, в том числе общий пользовательский календарь.

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    Успешный отклик включает код ответа HTTP 200 и коллекцию календарей, к которым Анна имеет доступ, в том числе календарь («Детские праздники») с именем владельца, указанным как "Артем Кузнецов", в качестве второго календаря. Для получателя общего доступа, Анны, свойство **canShare** общего календаря всегда имеет значение "false".

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
      "truncated": true,
      "@odata.type": "microsoft.graph.calendar",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json

    {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
        "value": [
            {
                "id": "AQMkADU5NAAAJMjAAAAA==",
                "name": "Calendar",
                "color": "auto",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
                "canShare": true,
                "canViewPrivateItems": true,
                "canEdit": true,
                "owner": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            {
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. Войдя в систему под именем Анны, получите общий календарь или одно или несколько событий общего календаря, используя в отклике идентификатор второго календаря с шага 1. Идентификаторы общего календаря и его события соответствуют локальной копии календаря Артема в почтовом ящике Анны.

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

В случае успешного выполнения вы получите отклик HTTP 200 ОК и запрошенное событие, события или календарь, которым Артем поделился с Анной.


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md)
- [Предоставление общего доступа к календарю или его делегирование в Outlook (предварительная версия)](outlook-share-or-delegate-calendar.md)
- [Зачем выполнять интеграцию с Календарем Outlook?](outlook-calendar-concept-overview.md)
- [API календаря](/graph/api/resources/calendar?view=graph-rest-1.0) в Microsoft Graph 1.0
