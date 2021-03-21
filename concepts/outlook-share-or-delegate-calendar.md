---
title: Предоставление общего доступа к календарю или его делегирование в Outlook
description: В Outlook владелец календаря может поделиться им с другим пользователем либо делегировать другому пользователю управление собраниями в основном календаре владельца.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 8bf08b8d32a53e5b309b2048060a8c64d1cb1ce7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962450"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a>Предоставление общего доступа к календарю или его делегирование в Outlook

В Outlook владелец календаря может поделиться им с другим пользователем. Владелец может указать, какие сведения об общедоступных событиях можно просматривать, а также может предоставить пользователям из той же организации доступ для записи к календарю. 

Владелец также может делегировать другому пользователю управление собраниями в _основном_ календаре владельца. Делегаты — это получатели общего доступа, которые могут просматривать все сведения и имеют доступ для записи к общедоступным событиям. Кроме того, они получают приглашения на собрания и ответы на них, а также отвечают на приглашения на собрания от имени владельца. Владелец также может предоставлять делегатам явные разрешения на просмотр _частных_ событий владельца в календаре. 

Перед предоставлением общего доступа к календарю или его делегированием владелец отправляет получателю общего доступа или делегату приглашение, а получатель общего доступа или делегат принимает приглашение или явным образом добавляет общий или делегированный календарь для доступа. Приглашение и добавление общего или делегированного календаря происходит в клиенте Outlook. 

После настройки общего доступа или делегирования в Outlook приложения смогут использовать API Microsoft Graph, чтобы управлять общим доступом и делегированием.

Оставшаяся часть этой статьи основана на следующем примере сценария:

- Алекс Уилбер (Alex Wilber) делегирует Меган Боуен (Megan Bowen) в свой основной календарь и разрешает ей просматривать частные события в этом календаре. 
- Алекс делится календарем "Детские праздники" с Адель Вэнс (Adele Vance) и Меган Боуен и предоставляет им обеим разрешения `read` для доступа ко всем сведениям об общедоступных событиях в календаре "Детские праздники", а также сведениям о доступности для частных событий. 

В этой статье описано, как программным способом выполнить следующие задачи в общем или делегированном календаре:

- [Получение сведений календаря о получателях общего доступа, делегатах и предоставленных разрешениях, а также обновление отдельных разрешений](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).
- [Получение свойств, описывающих общий доступ к календарю или его делегирование](#get-properties-of-a-shared-or-delegated-calendar).
- [Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них для делегированного календаря](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).
- [Удаление получателя общего доступа или делегата календаря](#delete-a-sharee-or-delegate-of-a-calendar).

Приложения также могут выполнять следующие задачи с помощью общедоступного API:

- [Получение общего или делегированного календаря Outlook или его событий](outlook-get-shared-events-calendars.md)
- [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md)

> [!NOTE]
> Свойства и API для общего доступа к календарям и их делегирования, как описано в этой статье, сейчас доступны в конечной точке версии 1.0, за исключением свойств календаря **isShared** и **isSharedWithMe**. Эти два свойства доступны только в конечной точке бета-версии.

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a>Получение сведений календаря о получателях общего доступа и делегатах, а также обновление отдельных разрешений

Содержание:

- [Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

Каждый календарь связан с коллекцией объектов [calendarPermission](/graph/api/resources/calendarpermission), каждый из которых описывает получателя общего доступа или делегата и соответствующее разрешение, настроенное владельцем календаря. Перечисление [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) определяет диапазон разрешений, поддерживаемых Microsoft Graph:

- `none`. Это значение применяется только к объекту `My Organization`, у которого нет никаких разрешений на доступ к календарю. Оно не применяется к отдельным пользователям, так как только пользователи с разрешениями связаны с объектом **calendarPermission** календаря.
- `freeBusyRead`. Получатель общего доступа может просматривать сведения о доступности владельца, но не другие сведения в календаре.
- `limitedRead`. Получатель общего доступа может просматривать сведения о доступности владельца, а также названия и расположения общедоступных событий календаря.
- `read`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также все сведения об общедоступных событиях календаря.
- `write`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также может просматривать все сведения и изменять (создавать, обновлять или удалять) общедоступные события календаря.
- `delegateWithoutPrivateEventAccess`. _Делегат_ может просматривать сведения о доступности владельца в частных событиях и обладает доступом с разрешением `write` к общедоступным событиям календаря.
- `delegateWithPrivateEventAccess`. _Делегат_ может просматривать сведения о частных и общедоступных событиях владельца и обладает доступом с разрешением `write` ко всем событиям календаря.

Основной календарь пользователя всегда предоставляется объекту My Organization (Моя организация), представляющему пользователей в организации владельца. По умолчанию они могут читать сведения о доступности владельца в этом календаре и обладают разрешением `freeBusyRead`.


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a>Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании

В этом примере показано, как с согласия Алекса или администратора получать объекты **calendarPermission**, связанные с основным календарем Алекса. Запрос возвращает два таких объекта разрешений:

- Первый объект **calendarPermission** присвоен делегату Меган со следующими значениями свойств:

  - Свойству **isRemovable** присвоено значение true, предоставляя Алексу возможность отменить делегирование.
  - Свойство **isInsideOrganization** имеет значение true, так как только пользователи из той же организации могут быть делегатами.
  - Свойству **role** для Меган соответствует значение `delegateWithPrivateEventAccess`, настроенное Алексом.
  - Свойство **allowedRoles** включает типы ролей `delegateWithoutPrivateEventAccess` и `delegateWithPrivateEventAccess`, поддерживающие делегирование.
  - **emailAddress** определяет Меган.

- Второй объект **calendarPermission** — это объект по умолчанию, назначаемый объекту My Organization со следующими значениями свойств:

  - Свойству **isRemovable** присвоено значение false, так как основной календарь всегда является общим для организации владельца.
  - Свойство **isInsideOrganization** имеет значение true.
  - Свойству **role** присвоено значение `freeBusyRead`, являющееся стандартным для объекта My Organization.
  - **emailAddress** определяет для дочернего свойства **name** значение My Organization; свойство **address** для My Organization по умолчанию имеет значение null.

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `Calendars.Read` соответственно. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarperms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendarperms",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/calendarPermissions",
    "value": [
        {
            "id": "L289RXhjaGFuZ2VMYWJTWVnYW5C",
            "isRemovable": true,
            "isInsideOrganization": true,
            "role": "delegateWithPrivateEventAccess",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read",
                "write",
                "delegateWithoutPrivateEventAccess",
                "delegateWithPrivateEventAccess"
            ],
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a>Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре

С согласия Алекса или администратора вы можете обновить разрешения, назначенные существующему получателю общего доступа или делегату (определяется свойством **role**), если новые разрешения поддерживаются свойством **allowedRoles**, настроенным изначально для получателя общего доступа или делегата для этого календаря. 

Кроме свойства **role**, вы не можете обновлять другие свойства существующего получателя общего доступа или делегата. Изменение значения свойства **emailAddress** требует удаления получателя общего доступа или делегата и повторной настройки нового экземпляра **calendarPermission**.

В примере из этого раздела обновляется свойство **role** с изменением разрешения существующего получателя общего доступа Адель с `read` на `write` для пользовательского календаря "Детские праздники".

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `Calendars.ReadWrite` соответственно. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarperm",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJQWRlbGVW"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarperm-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "update_calendarperm",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AAMkADAwAABf02bAAAA%3D')/calendarPermissions/$entity",
    "id": "L289RXhjaGFuZ2VMYWJQWRlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a>Получение свойств общего или делегированного календаря

Содержание:

- [Владелец календаря. Получение свойств общего или делегированного календаря](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

В этом примере Алекс делегировал свой основной календарь и предоставил делегату Меган Боуен разрешение на просмотр элементов календаря, помеченных как частные.
В этом разделе показаны свойства делегированного календаря, сначала с точки зрения и с согласия владельца (Алекс), а затем с точки зрения и с согласия делегата (Меган). Согласие администратора также поддерживается для каждого случая.

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a>Владелец календаря. Получение свойств общего или делегированного календаря

В примере из этого раздела выполняется получение свойств основного календаря с точки зрения владельца (Алекс). 

Обратите внимание на следующие свойства от имени Алекса:

- Свойство **canShare** имеет значение true, так как Алекс является владельцем.
- Свойство **canViewPrivateItems** имеет значение true, так как Алекс является владельцем.
- Свойству **isShared** присвоено значение true, так как Алекс настроил делегата для этого календаря.
- Свойство **isSharedWithMe** всегда имеет значение false для владельца календаря.
- Свойство **owner** отображает Алекса в качестве владельца.

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `Calendars.Read` соответственно. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAw7QAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a>Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря

В примере из этого раздела выполняется получение свойств того же календаря с точки зрения делегата (Меган). 

Обратите внимание на следующие свойства:

- Свойство **name** календаря по умолчанию соответствует отображаемому имени владельца. В этом случае это Alex Wilber (Алекс Уилбер), так как календарь Алекса делегирован Меган. 
- Свойство **canShare** имеет значение false, так как Меган не является владельцем этого календаря.
- Свойство **canViewPrivateItems** имеет значение true для делегата Меган, настроенное Алексом. Для получателя общего доступа, не являющегося делегатом, это свойство всегда имеет значение false.
- Свойство **isShared** имеет значение false. Это свойство указывает только для _владельца_ календаря, был ли к календарю предоставлен общий доступ или он был делегирован.
- Свойство **isSharedWithMe** имеет значение true, так как Меган является делегатом.
- Свойство **canEdit** имеет значение true, так как делегаты, включая Меган, обладают доступом с разрешением на запись.
- Свойству **owner** присвоено значение Alex (Алекс).

> [!NOTE] 
> Получатель общего доступа или делегат может настраивать только свойство **name** общего/делегированного календаря. Изменение отображается только для него самого. Владелец календаря не видит таких изменений имени календаря.

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами `Calendars.Read.Shared` или разрешением для приложений `Calendars.Read` соответственно. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-delegate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_delegate",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('meganb%40contoso.OnMicrosoft.com')/calendars/$entity",
    "id": "AAMkADlAABhbftjAAA=",
    "name": "Alex Wilber",
    "color": "auto",
    "hexColor": "",
    "changeKey": "E6LznKWmX0KTsAD9qRJjeAAAYWo3EQ==",
    "canShare": false,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": true,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a>Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них

Содержание:

- [Получение параметра доставки при делегировании для почтового ящика пользователя](#get-delegation-delivery-setting-for-a-users-mailbox)
- [Настройка параметра доставки при делегировании для почтового ящика пользователя](#set-delegation-delivery-setting-for-a-users-mailbox)

В зависимости от уровня делегирования, предпочитаемого владельцем календаря, владелец может указать, кто должен получать приглашения на собрания и ответы на них, чтобы управлять собраниями в календаре. 

Программным способом можно получить или настроить свойство **delegateMeetingMessageDeliveryOptions** объекта [mailboxSettings](/graph/api/resources/mailboxsettings) владельца календаря, чтобы указать, кому Outlook должен направлять экземпляры [eventMessageRequest](/graph/api/resources/eventmessagerequest) и [eventMessageResponse](/graph/api/resources/eventmessageresponse):

- `sendToDelegateOnly`

    Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** только делегатам. Это параметр по умолчанию. Владелец может просматривать ответы на приглашения на собрания или отвечать на приглашения с помощью соответствующего объекта **event** в делегированном календаре.
- `sendToDelegateAndInformationToPrincipal`

    Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря. Только делегатам доступны параметры для принятия и отклонения приглашения на собрание. Владельцу отправляется уведомление в виде обычного сообщения электронной почты. Владелец может ответить на приглашение, открыв объект **event** в делегированном календаре.
- `sendToDelegateAndPrincipal`

    Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря, любой из которых может ответить на приглашение на собрание.

Это параметр на уровне почтового ящика, поэтому этот параметр применяется ко всем делегатам владельца почтового ящика.

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a>Получение параметра доставки при делегировании для почтового ящика пользователя

В примере из этого раздела выполняется получение объекта **mailboxSettings** владельца календаря, который разрешает Outlook направлять приглашения на собрания и ответы на них только делегатам календаря. Таким образом, свойству **delegateMeetingMessageDeliveryOptions** присвоено значение `sendToDelegateOnly`.

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `MailboxSettings.Read` соответственно. Дополнительные сведения о разрешениях, необходимых для работы с почтовыми ящиками, см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "archiveFolder": "AQMkADAwAGVQAAAKfowAAAA==",
    "timeZone": "Pacific Standard Time",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly",
    "dateFormat": "M/d/yyyy",
    "timeFormat": "h:mm tt",
    "automaticRepliesSetting": {
        "status": "disabled",
        "externalAudience": "all",
        "internalReplyMessage": "",
        "externalReplyMessage": "",
        "scheduledStartDateTime": {
            "dateTime": "2019-12-24T05:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2019-12-25T05:00:00.0000000",
            "timeZone": "UTC"
        }
    },
    "language": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "workingHours": {
        "daysOfWeek": [
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone": {
            "name": "Pacific Standard Time"
        }
    }
}
```

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a>Настройка параметра доставки при делегировании для почтового ящика пользователя

В примере из этого раздела выполняется обновление свойства **delegateMeetingMessageDeliveryOptions** с присвоением ему значения `sendToDelegateAndPrincipal`, чтобы Outlook направлял приглашения на собрания и ответы на них в делегированном календаре всем делегатам и владельцу.

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `MailboxSettings.ReadWrite` соответственно. Дополнительные сведения о разрешениях, необходимых для работы с почтовыми ящиками, см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
Content-type: application/json

{
  "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "patch_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a>Удаление получателя общего доступа или делегата календаря

В примере ниже Алекс удаляет Меган из роли получателя общего доступа к календарю "Детские праздники".

**Разрешения Microsoft Graph**

Для выполнения этой операции воспользуйтесь делегированным разрешением с минимальными правами или разрешением для приложений `Calendars.ReadWrite` соответственно. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharee-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- Как клиенты Outlook поддерживают предоставление общего доступа к календарям и их делегирование:
  - [Предоставление общего доступа к календарю Outlook другим пользователям](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [Предоставление другому пользователю разрешения на управление собственной почтой и календарем в качестве делегата](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [Предоставление общего доступа к календарю в Outlook в Интернете](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [Делегирование доступа к календарю в Outlook в Интернете](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [Получение событий Outlook из общего или делегированного календаря](outlook-get-shared-events-calendars.md)
- [Создание событий Outlook в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md)
- [Зачем выполнять интеграцию с Календарем Outlook?](outlook-calendar-concept-overview.md)
- [API календаря](/graph/api/resources/calendar) в бета-версии Microsoft Graph.
