---
title: Предоставление общего доступа к календарю или его делегирование в Outlook
description: В Outlook владелец календаря может поделиться им с другим пользователем либо делегировать другому пользователю управление собраниями в основном календаре владельца.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 5e3db45879c062e4d7d8b247430a2595fe035632
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2020
ms.locfileid: "41656560"
---
# <a name="share-or-delegate-a-calendar-in-outlook-preview"></a><span data-ttu-id="697ca-103">Предоставление общего доступа к календарю или его делегирование в Outlook (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="697ca-103">Share or delegate a calendar in Outlook (preview)</span></span>

<span data-ttu-id="697ca-104">В Outlook владелец календаря может поделиться им с другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="697ca-104">In Outlook, a calendar owner can share the calendar with another user.</span></span> <span data-ttu-id="697ca-105">Владелец может указать, какие сведения об общедоступных событиях можно просматривать, а также может предоставить пользователям из той же организации доступ для записи к календарю.</span><span class="sxs-lookup"><span data-stu-id="697ca-105">The owner can specify which information in non-private events is viewable, and can give write access to the calendar to users in the same organization.</span></span> 

<span data-ttu-id="697ca-106">Владелец также может делегировать другому пользователю управление собраниями в _основном_ календаре владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-106">The owner can also delegate another user to manage meetings in the owner's _primary_ calendar.</span></span> <span data-ttu-id="697ca-107">Делегаты — это получатели общего доступа, которые могут просматривать все сведения и имеют доступ для записи к общедоступным событиям.</span><span class="sxs-lookup"><span data-stu-id="697ca-107">Delegates are sharees who can view all information in and have write access to non-private events.</span></span> <span data-ttu-id="697ca-108">Кроме того, они получают приглашения на собрания и ответы на них, а также отвечают на приглашения на собрания от имени владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-108">They also receive meeting requests and responses, and respond to meeting requests on behalf of the owner.</span></span> <span data-ttu-id="697ca-109">Владелец также может предоставлять делегатам явные разрешения на просмотр _частных_ событий владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-109">Additionally, the owner can give explicit permissions to delegates to view the owner's _private_ events on the calendar.</span></span> 

<span data-ttu-id="697ca-110">Перед предоставлением общего доступа к календарю или его делегированием владелец отправляет получателю общего доступа или делегату приглашение, а получатель общего доступа или делегат принимает приглашение или явным образом добавляет общий или делегированный календарь для доступа.</span><span class="sxs-lookup"><span data-stu-id="697ca-110">Before calendar sharing or delegation can take effect, the owner sends a sharee or delegate an invitation, and the sharee or delegate accepts the invitation, or, explicitly adds the shared or delegated calendar for access.</span></span> <span data-ttu-id="697ca-111">Приглашение и добавление общего или делегированного календаря происходит в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="697ca-111">The invitation and adding a shared or delegated calendar occur in an Outlook client.</span></span> 

<span data-ttu-id="697ca-112">После настройки общего доступа или делегирования в Outlook приложения смогут использовать API Microsoft Graph, чтобы управлять общим доступом и делегированием.</span><span class="sxs-lookup"><span data-stu-id="697ca-112">After sharing or delegation is set up in Outlook, apps can then use the Microsoft Graph API to manage the sharing and delegation.</span></span>

<span data-ttu-id="697ca-113">Оставшаяся часть этой статьи основана на следующем примере сценария:</span><span class="sxs-lookup"><span data-stu-id="697ca-113">The rest of this article is based on the following example scenario:</span></span>

- <span data-ttu-id="697ca-114">Алекс Уилбер (Alex Wilber) делегирует Меган Боуен (Megan Bowen) в свой основной календарь и разрешает ей просматривать частные события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-114">Alex Wilber has delegated Megan Bowen to his primary calendar, and also permitted Megan to view private events in that calendar.</span></span> 
- <span data-ttu-id="697ca-115">Алекс делится календарем "Детские праздники" с Адель Вэнс (Adele Vance) и Меган Боуен и предоставляет им обеим разрешения `read` для доступа ко всем сведениям об общедоступных событиях в календаре "Детские праздники", а также сведениям о доступности для частных событий.</span><span class="sxs-lookup"><span data-stu-id="697ca-115">Alex shared a "Kids parties" calendar with Adele Vance and Megan Bowen, and gave both Adele and Megan `read` permissions to all the details of non-private events on the "Kids parties" calendar, and free/busy status for private events.</span></span> 

<span data-ttu-id="697ca-116">В этой статье описано, как программным способом выполнить следующие задачи в общем или делегированном календаре:</span><span class="sxs-lookup"><span data-stu-id="697ca-116">This article describes programmatically carrying out the following tasks with a shared or delegated calendar:</span></span>

- <span data-ttu-id="697ca-117">[Получение сведений календаря о получателях общего доступа, делегатах и предоставленных разрешениях, а также обновление отдельных разрешений](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span><span class="sxs-lookup"><span data-stu-id="697ca-117">[Get calendar information about sharees, delegates, and allowed permissions, and update individual permissions](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span></span>
- <span data-ttu-id="697ca-118">[Получение свойств, описывающих общий доступ к календарю или его делегирование](#get-properties-of-a-shared-or-delegated-calendar).</span><span class="sxs-lookup"><span data-stu-id="697ca-118">[Get the properties that describe the sharing or delegation of the calendar](#get-properties-of-a-shared-or-delegated-calendar).</span></span>
- <span data-ttu-id="697ca-119">[Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них для делегированного календаря](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span><span class="sxs-lookup"><span data-stu-id="697ca-119">[Get or set mailbox setting to receive meeting requests and responses for a delegated calendar](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span></span>
- <span data-ttu-id="697ca-120">[Удаление получателя общего доступа или делегата календаря](#delete-a-sharee-or-delegate-of-a-calendar).</span><span class="sxs-lookup"><span data-stu-id="697ca-120">[Delete a sharee or delegate of a calendar](#delete-a-sharee-or-delegate-of-a-calendar).</span></span>

> [!NOTE]
> <span data-ttu-id="697ca-121">Указанные выше задачи используют API-интерфейс для общего доступа к календарю и его делегирования, который представлен [для ознакомления и доступен только в бета-версии](versioning-and-support.md#beta-version), за исключением следующих четырех свойств ресурса [calendar](/graph/api/resources/calendar?view=graph-rest-1.0): **canEdit**, **canShare**, **canViewPrivateItems** и **owner**.</span><span class="sxs-lookup"><span data-stu-id="697ca-121">The preceding tasks use API for calendar sharing and delegation that is [in preview and available only in the beta version](versioning-and-support.md#beta-version), with the exception of these four [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) properties: **canEdit**, **canShare**, **canViewPrivateItems**, and **owner**.</span></span>

<span data-ttu-id="697ca-122">Приложения также могут выполнять следующие задачи с помощью общедоступного API:</span><span class="sxs-lookup"><span data-stu-id="697ca-122">Apps can also do the following using API that is generally available:</span></span>

- [<span data-ttu-id="697ca-123">Получение общего или делегированного календаря Outlook или его событий</span><span class="sxs-lookup"><span data-stu-id="697ca-123">Get shared or delegated Outlook calendar or its events</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="697ca-124">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="697ca-124">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a><span data-ttu-id="697ca-125">Получение сведений календаря о получателях общего доступа и делегатах, а также обновление отдельных разрешений</span><span class="sxs-lookup"><span data-stu-id="697ca-125">Get calendar information about sharees and delegates, and update individual permissions</span></span>

<span data-ttu-id="697ca-126">Содержание:</span><span class="sxs-lookup"><span data-stu-id="697ca-126">In this section:</span></span>

- [<span data-ttu-id="697ca-127">Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании</span><span class="sxs-lookup"><span data-stu-id="697ca-127">Calendar owner: Get sharing or delegation information and permissions</span></span>](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [<span data-ttu-id="697ca-128">Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре</span><span class="sxs-lookup"><span data-stu-id="697ca-128">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

<span data-ttu-id="697ca-129">Каждый календарь связан с коллекцией объектов [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta), каждый из которых описывает получателя общего доступа или делегата и соответствующее разрешение, настроенное владельцем календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-129">Each calendar is associated with a collection of [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta) objects, each of which describes a sharee or delegate and the associated permission that the calendar owner has set up.</span></span> <span data-ttu-id="697ca-130">Перечисление [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values?view=graph-rest-beta) определяет диапазон разрешений, поддерживаемых Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="697ca-130">The [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values?view=graph-rest-beta) enumeration defines the range of permissions that Microsoft Graph supports:</span></span>

- <span data-ttu-id="697ca-131">`none`. Это значение применяется только к объекту `My Organization`, у которого нет никаких разрешений на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="697ca-131">`none` This value applies to only `My Organization` which does not have any permissions to the calendar.</span></span> <span data-ttu-id="697ca-132">Оно не применяется к отдельным пользователям, так как только пользователи с разрешениями связаны с объектом **calendarPermission** календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-132">It doesn't apply to individual users, as only users with permissions are associated with a **calendarPermission** object for the calendar.</span></span>
- <span data-ttu-id="697ca-133">`freeBusyRead`. Получатель общего доступа может просматривать сведения о доступности владельца, но не другие сведения в календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-133">`freeBusyRead` The sharee can view the owner's free/busy status, but not other details on the calendar.</span></span>
- <span data-ttu-id="697ca-134">`limitedRead`. Получатель общего доступа может просматривать сведения о доступности владельца, а также названия и расположения общедоступных событий календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-134">`limitedRead` The sharee can view the owner's free/busy status, and the titles and locations of non-private events on the calendar.</span></span>
- <span data-ttu-id="697ca-135">`read`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также все сведения об общедоступных событиях календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-135">`read` The sharee can view the owner's free/busy status in private events, and all the details of non-private events on the calendar.</span></span>
- <span data-ttu-id="697ca-136">`write`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также может просматривать все сведения и изменять (создавать, обновлять или удалять) общедоступные события календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-136">`write` The sharee can view the owner's free/busy status in private events, and can view all the details and edit (create, update, or delete) non-private events on the calendar.</span></span>
- <span data-ttu-id="697ca-137">`delegateWithoutPrivateEventAccess`. _Делегат_ может просматривать сведения о доступности владельца в частных событиях и обладает доступом с разрешением `write` к общедоступным событиям календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-137">`delegateWithoutPrivateEventAccess` The _delegate_ can view the owner's free/busy status in private events, and has `write` access to non-private events on the calendar.</span></span>
- <span data-ttu-id="697ca-138">`delegateWithPrivateEventAccess`. _Делегат_ может просматривать сведения о частных и общедоступных событиях владельца и обладает доступом с разрешением `write` ко всем событиям календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-138">`delegateWithPrivateEventAccess` The _delegate_ can view details of the owner's private and non-private events, and has `write` access to all the events on the calendar.</span></span>

<span data-ttu-id="697ca-139">Основной календарь пользователя всегда предоставляется объекту My Organization (Моя организация), представляющему пользователей в организации владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-139">The primary calendar of a user is always shared with "My Organization", which represents the users in the same organization as the owner.</span></span> <span data-ttu-id="697ca-140">По умолчанию они могут читать сведения о доступности владельца в этом календаре и обладают разрешением `freeBusyRead`.</span><span class="sxs-lookup"><span data-stu-id="697ca-140">By default, they can read the owner's free/busy status on that calendar and have the `freeBusyRead` permission.</span></span>


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a><span data-ttu-id="697ca-141">Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании</span><span class="sxs-lookup"><span data-stu-id="697ca-141">Calendar owner: Get sharing or delegation information and permissions</span></span>

<span data-ttu-id="697ca-142">В следующем примере показано, как с согласия Алекса или администратора получать объекты **calendarPermission**, связанные с основным календарем Алекса.</span><span class="sxs-lookup"><span data-stu-id="697ca-142">The following example shows with the consent of Alex or administrator, how to get the **calendarPermission** objects associated with Alex' primary calendar.</span></span> <span data-ttu-id="697ca-143">Запрос возвращает два таких объекта разрешений:</span><span class="sxs-lookup"><span data-stu-id="697ca-143">The request returns two such permission objects:</span></span>

- <span data-ttu-id="697ca-144">Первый объект **calendarPermission** присвоен делегату Меган со следующими значениями свойств:</span><span class="sxs-lookup"><span data-stu-id="697ca-144">The first **calendarPermission** object is assigned to the delegate, Megan, and has the following property values:</span></span>

  - <span data-ttu-id="697ca-145">Свойству **isRemovable** присвоено значение true, предоставляя Алексу возможность отменить делегирование.</span><span class="sxs-lookup"><span data-stu-id="697ca-145">**isRemovable** is set to true, providing Alex the option to cancel the delegation.</span></span>
  - <span data-ttu-id="697ca-146">Свойство **isInsideOrganization** имеет значение true, так как только пользователи из той же организации могут быть делегатами.</span><span class="sxs-lookup"><span data-stu-id="697ca-146">**isInsideOrganization** is true as only users in the same organization can be delegates.</span></span>
  - <span data-ttu-id="697ca-147">Свойству **role** для Меган соответствует значение `delegateWithPrivateEventAccess`, настроенное Алексом.</span><span class="sxs-lookup"><span data-stu-id="697ca-147">**role** for Megan is `delegateWithPrivateEventAccess`, as set up by Alex.</span></span>
  - <span data-ttu-id="697ca-148">Свойство **allowedRoles** включает типы ролей `delegateWithoutPrivateEventAccess` и `delegateWithPrivateEventAccess`, поддерживающие делегирование.</span><span class="sxs-lookup"><span data-stu-id="697ca-148">**allowedRoles** includes the role types `delegateWithoutPrivateEventAccess` and `delegateWithPrivateEventAccess` that support delegation.</span></span>
  - <span data-ttu-id="697ca-149">**emailAddress** определяет Меган.</span><span class="sxs-lookup"><span data-stu-id="697ca-149">**emailAddress** specifies Megan.</span></span>

- <span data-ttu-id="697ca-150">Второй объект **calendarPermission** — это объект по умолчанию, назначаемый объекту My Organization со следующими значениями свойств:</span><span class="sxs-lookup"><span data-stu-id="697ca-150">The second **calendarPermission** object is a default object assigned to "My Organization", and has the following property values:</span></span>

  - <span data-ttu-id="697ca-151">Свойству **isRemovable** присвоено значение false, так как основной календарь всегда является общим для организации владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-151">**isRemovable** is set to false, since the primary calendar is always shared with the owner's organization.</span></span>
  - <span data-ttu-id="697ca-152">Свойство **isInsideOrganization** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="697ca-152">**isInsideOrganization** is true.</span></span>
  - <span data-ttu-id="697ca-153">Свойству **role** присвоено значение `freeBusyRead`, являющееся стандартным для объекта My Organization.</span><span class="sxs-lookup"><span data-stu-id="697ca-153">**role** is `freeBusyRead`, the default setting for "My Organization".</span></span>
  - <span data-ttu-id="697ca-154">**emailAddress** определяет для дочернего свойства **name** значение My Organization; свойство **address** для My Organization по умолчанию имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="697ca-154">**emailAddress** specifies the **name** sub-property as "My Organization"; **address** for "My Organization" is by default null.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```http
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```

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


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a><span data-ttu-id="697ca-155">Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре</span><span class="sxs-lookup"><span data-stu-id="697ca-155">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>

<span data-ttu-id="697ca-156">С согласия Алекса или администратора вы можете обновить разрешения, назначенные существующему получателю общего доступа или делегату (определяется свойством **role**), если новые разрешения поддерживаются свойством **allowedRoles**, настроенным изначально для получателя общего доступа или делегата для этого календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-156">With the consent of Alex or administrator, you can update the permissions assigned to an existing sharee or delegate (specified by the **role** property), as long as the new permissions are supported by those **allowedRoles** set up initially for the sharee or delegate for that calendar.</span></span> 

<span data-ttu-id="697ca-157">Кроме свойства **role**, вы не можете обновлять другие свойства существующего получателя общего доступа или делегата.</span><span class="sxs-lookup"><span data-stu-id="697ca-157">Aside from the **role** property, you cannot update other properties of an existing sharee or delegate.</span></span> <span data-ttu-id="697ca-158">Изменение значения свойства **emailAddress** требует удаления получателя общего доступа или делегата и повторной настройки нового экземпляра **calendarPermission**.</span><span class="sxs-lookup"><span data-stu-id="697ca-158">Changing the **emailAddress** property value requires deleting the sharee or delegate and setting up a new instance of **calendarPermission** again.</span></span>

<span data-ttu-id="697ca-159">В следующем примере обновляется свойство **role** с изменением разрешения существующего получателя общего доступа Адель с `read` на `write` для пользовательского календаря "Детские праздники".</span><span class="sxs-lookup"><span data-stu-id="697ca-159">The following example updates the **role** property, changing the permission of an existing sharee, Adele, from `read` to `write` for the custom calendar "Kids parties".</span></span>

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


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="697ca-160">Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-160">Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="697ca-161">Содержание:</span><span class="sxs-lookup"><span data-stu-id="697ca-161">In this section:</span></span>

- [<span data-ttu-id="697ca-162">Владелец календаря. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-162">Calendar owner: Get properties of a shared or delegated calendar</span></span>](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [<span data-ttu-id="697ca-163">Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-163">Sharee or delegate: Get properties of shared or delegated calendar</span></span>](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

<span data-ttu-id="697ca-164">В этом примере Алекс делегировал свой основной календарь и предоставил делегату Меган Боуен разрешение на просмотр элементов календаря, помеченных как частные.</span><span class="sxs-lookup"><span data-stu-id="697ca-164">Recalling in this example, Alex has delegated his primary calendar and given the delegate, Megan Bowen, the permission to view calendar items that are marked private.</span></span>
<span data-ttu-id="697ca-165">В этом разделе показаны свойства делегированного календаря, сначала с точки зрения и с согласия владельца (Алекс), а затем с точки зрения и с согласия делегата (Меган).</span><span class="sxs-lookup"><span data-stu-id="697ca-165">This section shows the properties of the delegated calendar, first from the perspective of and with the consent of the owner, Alex, and then from the perspective of and with the consent of the delegate, Megan.</span></span> <span data-ttu-id="697ca-166">Согласие администратора также поддерживается для каждого случая.</span><span class="sxs-lookup"><span data-stu-id="697ca-166">Consent from the administrator also works for each case.</span></span>

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="697ca-167">Владелец календаря. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-167">Calendar owner: Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="697ca-168">В следующем примере выполняется получение свойств основного календаря с точки зрения владельца (Алекс).</span><span class="sxs-lookup"><span data-stu-id="697ca-168">The following example gets the properties of the primary calendar from the perspective of the owner, Alex.</span></span> 

<span data-ttu-id="697ca-169">Обратите внимание на следующие свойства от имени Алекса:</span><span class="sxs-lookup"><span data-stu-id="697ca-169">Note the following properties on Alex' behalf:</span></span>

- <span data-ttu-id="697ca-170">Свойство **canShare** имеет значение true, так как Алекс является владельцем.</span><span class="sxs-lookup"><span data-stu-id="697ca-170">**canShare** is true as Alex is the owner.</span></span>
- <span data-ttu-id="697ca-171">Свойство **canViewPrivateItems** имеет значение true, так как Алекс является владельцем.</span><span class="sxs-lookup"><span data-stu-id="697ca-171">**canViewPrivateItems** is true since Alex is the owner.</span></span>
- <span data-ttu-id="697ca-172">Свойству **isShared** присвоено значение true, так как Алекс настроил делегата для этого календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-172">**isShared** is set to true, as Alex has set up a delegate for this calendar.</span></span>
- <span data-ttu-id="697ca-173">Свойство **isSharedWithMe** всегда имеет значение false для владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-173">**isSharedWithMe** is always false for the calendar owner.</span></span>
- <span data-ttu-id="697ca-174">Свойство **owner** отображает Алекса в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-174">**owner** shows Alex as the owner.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```

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
    "isDefaultCalendar": true,
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


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a><span data-ttu-id="697ca-175">Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-175">Sharee or delegate: Get properties of shared or delegated calendar</span></span>

<span data-ttu-id="697ca-176">В следующем примере выполняется получение свойств того же календаря с точки зрения делегата (Меган).</span><span class="sxs-lookup"><span data-stu-id="697ca-176">The following example gets the properties of the same calendar from the perspective of the delegate, Megan.</span></span> 

<span data-ttu-id="697ca-177">Обратите внимание на следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="697ca-177">Note the following properties:</span></span>

- <span data-ttu-id="697ca-178">Свойство **name** календаря по умолчанию соответствует отображаемому имени владельца.</span><span class="sxs-lookup"><span data-stu-id="697ca-178">**name** of the calendar is by default the owner's display name.</span></span> <span data-ttu-id="697ca-179">В этом случае это Alex Wilber (Алекс Уилбер), так как календарь Алекса делегирован Меган.</span><span class="sxs-lookup"><span data-stu-id="697ca-179">In this case, it's "Alex Wilber", since this is Alex' calendar delegated to Megan.</span></span> 
- <span data-ttu-id="697ca-180">Свойство **canShare** имеет значение false, так как Меган не является владельцем этого календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-180">**canShare** is false, since Megan is not the owner of this calendar.</span></span>
- <span data-ttu-id="697ca-181">Свойство **canViewPrivateItems** имеет значение true для делегата Меган, настроенное Алексом.</span><span class="sxs-lookup"><span data-stu-id="697ca-181">**canViewPrivateItems** is true for the delegate Megan, as set up by Alex.</span></span> <span data-ttu-id="697ca-182">Для получателя общего доступа, не являющегося делегатом, это свойство всегда имеет значение false.</span><span class="sxs-lookup"><span data-stu-id="697ca-182">For a sharee that is not a delegate, this property is always false.</span></span>
- <span data-ttu-id="697ca-183">Свойство **isShared** имеет значение false.</span><span class="sxs-lookup"><span data-stu-id="697ca-183">**isShared** is false.</span></span> <span data-ttu-id="697ca-184">Это свойство указывает только для _владельца_ календаря, был ли к календарю предоставлен общий доступ или он был делегирован.</span><span class="sxs-lookup"><span data-stu-id="697ca-184">This property indicates only to a calendar _owner_ whether the calendar has been shared or delegated.</span></span>
- <span data-ttu-id="697ca-185">Свойство **isSharedWithMe** имеет значение true, так как Меган является делегатом.</span><span class="sxs-lookup"><span data-stu-id="697ca-185">**isSharedWithMe** property is true, since Megan is a delegate.</span></span>
- <span data-ttu-id="697ca-186">Свойство **canEdit** имеет значение true, так как делегаты, включая Меган, обладают доступом с разрешением на запись.</span><span class="sxs-lookup"><span data-stu-id="697ca-186">**canEdit** is true, since delegates, including Megan, have write access.</span></span>
- <span data-ttu-id="697ca-187">Свойству **owner** присвоено значение Alex (Алекс).</span><span class="sxs-lookup"><span data-stu-id="697ca-187">**owner** is set to Alex.</span></span>

> [!NOTE] 
> <span data-ttu-id="697ca-188">Получатель общего доступа или делегат может настраивать только свойство **name** общего/делегированного календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-188">A sharee or delegate can customize only the **name** property of a shared/delegated calendar.</span></span> <span data-ttu-id="697ca-189">Изменение отображается только для него самого. Владелец календаря не видит таких изменений имени календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-189">The update is visible only to themselves; the calendar owner does not see such calendar name changes.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```http
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```

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
    "isDefaultCalendar": false,
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


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a><span data-ttu-id="697ca-190">Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них</span><span class="sxs-lookup"><span data-stu-id="697ca-190">Get or set mailbox setting to receive meeting requests and responses</span></span>

<span data-ttu-id="697ca-191">Содержание:</span><span class="sxs-lookup"><span data-stu-id="697ca-191">In this section:</span></span>

- [<span data-ttu-id="697ca-192">Получение параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="697ca-192">Get delegation delivery setting for a user's mailbox</span></span>](#get-delegation-delivery-setting-for-a-users-mailbox)
- [<span data-ttu-id="697ca-193">Настройка параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="697ca-193">Set delegation delivery setting for a user's mailbox</span></span>](#set-delegation-delivery-setting-for-a-users-mailbox)

<span data-ttu-id="697ca-194">В зависимости от уровня делегирования, предпочитаемого владельцем календаря, владелец может указать, кто должен получать приглашения на собрания и ответы на них, чтобы управлять собраниями в календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-194">Depending on the level of delegation a calendar owner prefers, the owner can specify who should receive meeting requests and responses to manage meetings on the calendar.</span></span> 

<span data-ttu-id="697ca-195">Программным способом можно получить или настроить свойство **delegateMeetingMessageDeliveryOptions** объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) владельца календаря, чтобы указать, кому Outlook должен направлять экземпляры [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-beta) и [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-beta):</span><span class="sxs-lookup"><span data-stu-id="697ca-195">Programmatically, you can get or set the **delegateMeetingMessageDeliveryOptions** property of the calendar owner's [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) to specify to whom Outlook should direct [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-beta) and [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-beta) instances:</span></span>

- `sendToDelegateOnly`

    <span data-ttu-id="697ca-196">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** только делегатам.</span><span class="sxs-lookup"><span data-stu-id="697ca-196">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to only delegates.</span></span> <span data-ttu-id="697ca-197">Это параметр по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="697ca-197">This is the default setting.</span></span> <span data-ttu-id="697ca-198">Владелец может просматривать ответы на приглашения на собрания или отвечать на приглашения с помощью соответствующего объекта **event** в делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-198">The owner can see responses to a meeting or respond to an invitation through the corresponding **event** in the delegated calendar.</span></span>
- `sendToDelegateAndInformationToPrincipal`

    <span data-ttu-id="697ca-199">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря.</span><span class="sxs-lookup"><span data-stu-id="697ca-199">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner.</span></span> <span data-ttu-id="697ca-200">Только делегатам доступны параметры для принятия и отклонения приглашения на собрание. Владельцу отправляется уведомление в виде обычного сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="697ca-200">Only the delegates see the option to accept or decline a meeting request, and the notification sent to the owner appears like a normal email message.</span></span> <span data-ttu-id="697ca-201">Владелец может ответить на приглашение, открыв объект **event** в делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="697ca-201">The owner can still respond to the meeting by opening the **event** in the delegated calendar and responding.</span></span>
- `sendToDelegateAndPrincipal`

    <span data-ttu-id="697ca-202">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря, любой из которых может ответить на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="697ca-202">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner, either of whom can respond to the meeting request.</span></span>

<span data-ttu-id="697ca-203">Это параметр на уровне почтового ящика, поэтому этот параметр применяется ко всем делегатам владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="697ca-203">This is a mailbox-wide setting, so the same setting applies to all delegates of the mailbox owner.</span></span>

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="697ca-204">Получение параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="697ca-204">Get delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="697ca-205">В следующем примере выполняется получение объекта **mailboxSettings** владельца календаря, который разрешает Outlook направлять приглашения на собрания и ответы на них только делегатам календаря. Таким образом, свойству **delegateMeetingMessageDeliveryOptions** присвоено значение `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="697ca-205">The following example gets the **mailboxSettings** of a calendar owner who lets Outlook direct meeting requests and responses to only calendar delegates; that is, **delegateMeetingMessageDeliveryOptions** is set to `sendToDelegateOnly`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```

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

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="697ca-206">Настройка параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="697ca-206">Set delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="697ca-207">В следующем примере выполняется обновление свойства **delegateMeetingMessageDeliveryOptions** с присвоением ему значения `sendToDelegateAndPrincipal`, чтобы Outlook направлял приглашения на собрания и ответы на них в делегированном календаре всем делегатам и владельцу.</span><span class="sxs-lookup"><span data-stu-id="697ca-207">The following example updates the **delegateMeetingMessageDeliveryOptions** property to `sendToDelegateAndPrincipal`, to have Outlook direct meeting requests and responses of the delegated calendar to all delegates and the owner.</span></span>

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


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a><span data-ttu-id="697ca-208">Удаление получателя общего доступа или делегата календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-208">Delete a sharee or delegate of a calendar</span></span>

<span data-ttu-id="697ca-209">В следующем примере Алекс удаляет Меган из роли получателя общего доступа к календарю "Детские праздники".</span><span class="sxs-lookup"><span data-stu-id="697ca-209">In the following example, Alex deletes Megan as a sharee of the "Kids parties" calendar.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```

<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a><span data-ttu-id="697ca-210">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="697ca-210">Next steps</span></span>

<span data-ttu-id="697ca-211">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="697ca-211">Find out more about:</span></span>

- <span data-ttu-id="697ca-212">Как клиенты Outlook поддерживают предоставление общего доступа к календарям и их делегирование:</span><span class="sxs-lookup"><span data-stu-id="697ca-212">How the Outlook clients support sharing and delegating calendars:</span></span>
  - [<span data-ttu-id="697ca-213">Предоставление общего доступа к календарю Outlook другим пользователям</span><span class="sxs-lookup"><span data-stu-id="697ca-213">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [<span data-ttu-id="697ca-214">Предоставление другому пользователю разрешения на управление собственной почтой и календарем в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="697ca-214">Allow someone else to manage your mail and calendar as a delegate</span></span>](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [<span data-ttu-id="697ca-215">Предоставление общего доступа к календарю в Outlook в Интернете</span><span class="sxs-lookup"><span data-stu-id="697ca-215">Share your calendar in Outlook on the web</span></span>](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [<span data-ttu-id="697ca-216">Делегирование доступа к календарю в Outlook в Интернете</span><span class="sxs-lookup"><span data-stu-id="697ca-216">Calendar delegation in Outlook on the web</span></span>](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [<span data-ttu-id="697ca-217">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="697ca-217">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="697ca-218">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="697ca-218">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="697ca-219">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="697ca-219">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="697ca-220">[API календаря](/graph/api/resources/calendar?view=graph-rest-beta) в бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="697ca-220">The [calendar API](/graph/api/resources/calendar?view=graph-rest-beta) in Microsoft Graph beta.</span></span>