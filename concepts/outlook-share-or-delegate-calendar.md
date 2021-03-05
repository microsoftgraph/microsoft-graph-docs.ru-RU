---
title: Предоставление общего доступа к календарю или его делегирование в Outlook
description: В Outlook владелец календаря может поделиться им с другим пользователем либо делегировать другому пользователю управление собраниями в основном календаре владельца.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: f04b1138fe8967a682ba890a5947c4e861c47717
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474941"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a><span data-ttu-id="1064d-103">Предоставление общего доступа к календарю или его делегирование в Outlook</span><span class="sxs-lookup"><span data-stu-id="1064d-103">Share or delegate a calendar in Outlook</span></span>

<span data-ttu-id="1064d-104">В Outlook владелец календаря может поделиться им с другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="1064d-104">In Outlook, a calendar owner can share the calendar with another user.</span></span> <span data-ttu-id="1064d-105">Владелец может указать, какие сведения об общедоступных событиях можно просматривать, а также может предоставить пользователям из той же организации доступ для записи к календарю.</span><span class="sxs-lookup"><span data-stu-id="1064d-105">The owner can specify which information in non-private events is viewable, and can give write access to the calendar to users in the same organization.</span></span> 

<span data-ttu-id="1064d-106">Владелец также может делегировать другому пользователю управление собраниями в _основном_ календаре владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-106">The owner can also delegate another user to manage meetings in the owner's _primary_ calendar.</span></span> <span data-ttu-id="1064d-107">Делегаты — это получатели общего доступа, которые могут просматривать все сведения и имеют доступ для записи к общедоступным событиям.</span><span class="sxs-lookup"><span data-stu-id="1064d-107">Delegates are sharees who can view all information in and have write access to non-private events.</span></span> <span data-ttu-id="1064d-108">Кроме того, они получают приглашения на собрания и ответы на них, а также отвечают на приглашения на собрания от имени владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-108">They also receive meeting requests and responses, and respond to meeting requests on behalf of the owner.</span></span> <span data-ttu-id="1064d-109">Владелец также может предоставлять делегатам явные разрешения на просмотр _частных_ событий владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-109">Additionally, the owner can give explicit permissions to delegates to view the owner's _private_ events on the calendar.</span></span> 

<span data-ttu-id="1064d-110">Перед предоставлением общего доступа к календарю или его делегированием владелец отправляет получателю общего доступа или делегату приглашение, а получатель общего доступа или делегат принимает приглашение или явным образом добавляет общий или делегированный календарь для доступа.</span><span class="sxs-lookup"><span data-stu-id="1064d-110">Before calendar sharing or delegation can take effect, the owner sends a sharee or delegate an invitation, and the sharee or delegate accepts the invitation, or, explicitly adds the shared or delegated calendar for access.</span></span> <span data-ttu-id="1064d-111">Приглашение и добавление общего или делегированного календаря происходит в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="1064d-111">The invitation and adding a shared or delegated calendar occur in an Outlook client.</span></span> 

<span data-ttu-id="1064d-112">После настройки общего доступа или делегирования в Outlook приложения смогут использовать API Microsoft Graph, чтобы управлять общим доступом и делегированием.</span><span class="sxs-lookup"><span data-stu-id="1064d-112">After sharing or delegation is set up in Outlook, apps can then use the Microsoft Graph API to manage the sharing and delegation.</span></span>

<span data-ttu-id="1064d-113">Оставшаяся часть этой статьи основана на следующем примере сценария:</span><span class="sxs-lookup"><span data-stu-id="1064d-113">The rest of this article is based on the following example scenario:</span></span>

- <span data-ttu-id="1064d-114">Алекс Уилбер (Alex Wilber) делегирует Меган Боуен (Megan Bowen) в свой основной календарь и разрешает ей просматривать частные события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-114">Alex Wilber has delegated Megan Bowen to his primary calendar, and also permitted Megan to view private events in that calendar.</span></span> 
- <span data-ttu-id="1064d-115">Алекс делится календарем "Детские праздники" с Адель Вэнс (Adele Vance) и Меган Боуен и предоставляет им обеим разрешения `read` для доступа ко всем сведениям об общедоступных событиях в календаре "Детские праздники", а также сведениям о доступности для частных событий.</span><span class="sxs-lookup"><span data-stu-id="1064d-115">Alex shared a "Kids parties" calendar with Adele Vance and Megan Bowen, and gave both Adele and Megan `read` permissions to all the details of non-private events on the "Kids parties" calendar, and free/busy status for private events.</span></span> 

<span data-ttu-id="1064d-116">В этой статье описано, как программным способом выполнить следующие задачи в общем или делегированном календаре:</span><span class="sxs-lookup"><span data-stu-id="1064d-116">This article describes programmatically carrying out the following tasks with a shared or delegated calendar:</span></span>

- <span data-ttu-id="1064d-117">[Получение сведений календаря о получателях общего доступа, делегатах и предоставленных разрешениях, а также обновление отдельных разрешений](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-117">[Get calendar information about sharees, delegates, and allowed permissions, and update individual permissions](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span></span>
- <span data-ttu-id="1064d-118">[Получение свойств, описывающих общий доступ к календарю или его делегирование](#get-properties-of-a-shared-or-delegated-calendar).</span><span class="sxs-lookup"><span data-stu-id="1064d-118">[Get the properties that describe the sharing or delegation of the calendar](#get-properties-of-a-shared-or-delegated-calendar).</span></span>
- <span data-ttu-id="1064d-119">[Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них для делегированного календаря](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span><span class="sxs-lookup"><span data-stu-id="1064d-119">[Get or set mailbox setting to receive meeting requests and responses for a delegated calendar](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span></span>
- <span data-ttu-id="1064d-120">[Удаление получателя общего доступа или делегата календаря](#delete-a-sharee-or-delegate-of-a-calendar).</span><span class="sxs-lookup"><span data-stu-id="1064d-120">[Delete a sharee or delegate of a calendar](#delete-a-sharee-or-delegate-of-a-calendar).</span></span>

<span data-ttu-id="1064d-121">Приложения также могут выполнять следующие задачи с помощью общедоступного API:</span><span class="sxs-lookup"><span data-stu-id="1064d-121">Apps can also do the following using API that is generally available:</span></span>

- [<span data-ttu-id="1064d-122">Получение общего или делегированного календаря Outlook или его событий</span><span class="sxs-lookup"><span data-stu-id="1064d-122">Get shared or delegated Outlook calendar or its events</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="1064d-123">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="1064d-123">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)

> [!NOTE]
> <span data-ttu-id="1064d-124">Свойства и API для общего доступа к календарям и их делегирования, как описано в этой статье, сейчас доступны в конечной точке версии 1.0, за исключением свойств календаря **isShared** и **isSharedWithMe**.</span><span class="sxs-lookup"><span data-stu-id="1064d-124">The properties and API for calendar sharing and delegating as described in this topic are currently available in the v1.0 endpoint, with the exception of the calendar properties **isShared** and **isSharedWithMe**.</span></span> <span data-ttu-id="1064d-125">Эти два свойства доступны только в конечной точке бета-версии.</span><span class="sxs-lookup"><span data-stu-id="1064d-125">These two properties are exposed in only the beta endpoint.</span></span>

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a><span data-ttu-id="1064d-126">Получение сведений календаря о получателях общего доступа и делегатах, а также обновление отдельных разрешений</span><span class="sxs-lookup"><span data-stu-id="1064d-126">Get calendar information about sharees and delegates, and update individual permissions</span></span>

<span data-ttu-id="1064d-127">Содержание:</span><span class="sxs-lookup"><span data-stu-id="1064d-127">In this section:</span></span>

- [<span data-ttu-id="1064d-128">Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании</span><span class="sxs-lookup"><span data-stu-id="1064d-128">Calendar owner: Get sharing or delegation information and permissions</span></span>](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [<span data-ttu-id="1064d-129">Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре</span><span class="sxs-lookup"><span data-stu-id="1064d-129">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

<span data-ttu-id="1064d-130">Каждый календарь связан с коллекцией объектов [calendarPermission](/graph/api/resources/calendarpermission), каждый из которых описывает получателя общего доступа или делегата и соответствующее разрешение, настроенное владельцем календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-130">Each calendar is associated with a collection of [calendarPermission](/graph/api/resources/calendarpermission) objects, each of which describes a sharee or delegate and the associated permission that the calendar owner has set up.</span></span> <span data-ttu-id="1064d-131">Перечисление [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) определяет диапазон разрешений, поддерживаемых Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="1064d-131">The [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) enumeration defines the range of permissions that Microsoft Graph supports:</span></span>

- <span data-ttu-id="1064d-132">`none`. Это значение применяется только к объекту `My Organization`, у которого нет никаких разрешений на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="1064d-132">`none` This value applies to only `My Organization` which does not have any permissions to the calendar.</span></span> <span data-ttu-id="1064d-133">Оно не применяется к отдельным пользователям, так как только пользователи с разрешениями связаны с объектом **calendarPermission** календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-133">It doesn't apply to individual users, as only users with permissions are associated with a **calendarPermission** object for the calendar.</span></span>
- <span data-ttu-id="1064d-134">`freeBusyRead`. Получатель общего доступа может просматривать сведения о доступности владельца, но не другие сведения в календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-134">`freeBusyRead` The sharee can view the owner's free/busy status, but not other details on the calendar.</span></span>
- <span data-ttu-id="1064d-135">`limitedRead`. Получатель общего доступа может просматривать сведения о доступности владельца, а также названия и расположения общедоступных событий календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-135">`limitedRead` The sharee can view the owner's free/busy status, and the titles and locations of non-private events on the calendar.</span></span>
- <span data-ttu-id="1064d-136">`read`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также все сведения об общедоступных событиях календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-136">`read` The sharee can view the owner's free/busy status in private events, and all the details of non-private events on the calendar.</span></span>
- <span data-ttu-id="1064d-137">`write`. Получатель общего доступа может просматривать сведения о доступности владельца в частных событиях, а также может просматривать все сведения и изменять (создавать, обновлять или удалять) общедоступные события календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-137">`write` The sharee can view the owner's free/busy status in private events, and can view all the details and edit (create, update, or delete) non-private events on the calendar.</span></span>
- <span data-ttu-id="1064d-138">`delegateWithoutPrivateEventAccess`. _Делегат_ может просматривать сведения о доступности владельца в частных событиях и обладает доступом с разрешением `write` к общедоступным событиям календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-138">`delegateWithoutPrivateEventAccess` The _delegate_ can view the owner's free/busy status in private events, and has `write` access to non-private events on the calendar.</span></span>
- <span data-ttu-id="1064d-139">`delegateWithPrivateEventAccess`. _Делегат_ может просматривать сведения о частных и общедоступных событиях владельца и обладает доступом с разрешением `write` ко всем событиям календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-139">`delegateWithPrivateEventAccess` The _delegate_ can view details of the owner's private and non-private events, and has `write` access to all the events on the calendar.</span></span>

<span data-ttu-id="1064d-140">Основной календарь пользователя всегда предоставляется объекту My Organization (Моя организация), представляющему пользователей в организации владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-140">The primary calendar of a user is always shared with "My Organization", which represents the users in the same organization as the owner.</span></span> <span data-ttu-id="1064d-141">По умолчанию они могут читать сведения о доступности владельца в этом календаре и обладают разрешением `freeBusyRead`.</span><span class="sxs-lookup"><span data-stu-id="1064d-141">By default, they can read the owner's free/busy status on that calendar and have the `freeBusyRead` permission.</span></span>


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a><span data-ttu-id="1064d-142">Владелец календаря. Получение разрешений и сведений об общем доступе или делегировании</span><span class="sxs-lookup"><span data-stu-id="1064d-142">Calendar owner: Get sharing or delegation information and permissions</span></span>

<span data-ttu-id="1064d-143">В этом примере показано, как с согласия Алекса или администратора получать объекты **calendarPermission**, связанные с основным календарем Алекса.</span><span class="sxs-lookup"><span data-stu-id="1064d-143">This example shows with the consent of Alex or administrator, how to get the **calendarPermission** objects associated with Alex' primary calendar.</span></span> <span data-ttu-id="1064d-144">Запрос возвращает два таких объекта разрешений:</span><span class="sxs-lookup"><span data-stu-id="1064d-144">The request returns two such permission objects:</span></span>

- <span data-ttu-id="1064d-145">Первый объект **calendarPermission** присвоен делегату Меган со следующими значениями свойств:</span><span class="sxs-lookup"><span data-stu-id="1064d-145">The first **calendarPermission** object is assigned to the delegate, Megan, and has the following property values:</span></span>

  - <span data-ttu-id="1064d-146">Свойству **isRemovable** присвоено значение true, предоставляя Алексу возможность отменить делегирование.</span><span class="sxs-lookup"><span data-stu-id="1064d-146">**isRemovable** is set to true, providing Alex the option to cancel the delegation.</span></span>
  - <span data-ttu-id="1064d-147">Свойство **isInsideOrganization** имеет значение true, так как только пользователи из той же организации могут быть делегатами.</span><span class="sxs-lookup"><span data-stu-id="1064d-147">**isInsideOrganization** is true as only users in the same organization can be delegates.</span></span>
  - <span data-ttu-id="1064d-148">Свойству **role** для Меган соответствует значение `delegateWithPrivateEventAccess`, настроенное Алексом.</span><span class="sxs-lookup"><span data-stu-id="1064d-148">**role** for Megan is `delegateWithPrivateEventAccess`, as set up by Alex.</span></span>
  - <span data-ttu-id="1064d-149">Свойство **allowedRoles** включает типы ролей `delegateWithoutPrivateEventAccess` и `delegateWithPrivateEventAccess`, поддерживающие делегирование.</span><span class="sxs-lookup"><span data-stu-id="1064d-149">**allowedRoles** includes the role types `delegateWithoutPrivateEventAccess` and `delegateWithPrivateEventAccess` that support delegation.</span></span>
  - <span data-ttu-id="1064d-150">**emailAddress** определяет Меган.</span><span class="sxs-lookup"><span data-stu-id="1064d-150">**emailAddress** specifies Megan.</span></span>

- <span data-ttu-id="1064d-151">Второй объект **calendarPermission** — это объект по умолчанию, назначаемый объекту My Organization со следующими значениями свойств:</span><span class="sxs-lookup"><span data-stu-id="1064d-151">The second **calendarPermission** object is a default object assigned to "My Organization", and has the following property values:</span></span>

  - <span data-ttu-id="1064d-152">Свойству **isRemovable** присвоено значение false, так как основной календарь всегда является общим для организации владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-152">**isRemovable** is set to false, since the primary calendar is always shared with the owner's organization.</span></span>
  - <span data-ttu-id="1064d-153">Свойство **isInsideOrganization** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="1064d-153">**isInsideOrganization** is true.</span></span>
  - <span data-ttu-id="1064d-154">Свойству **role** присвоено значение `freeBusyRead`, являющееся стандартным для объекта My Organization.</span><span class="sxs-lookup"><span data-stu-id="1064d-154">**role** is `freeBusyRead`, the default setting for "My Organization".</span></span>
  - <span data-ttu-id="1064d-155">**emailAddress** определяет для дочернего свойства **name** значение My Organization; свойство **address** для My Organization по умолчанию имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="1064d-155">**emailAddress** specifies the **name** sub-property as "My Organization"; **address** for "My Organization" is by default null.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-156">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-156">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-157">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `Calendars.Read` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-157">Use the least privileged delegated or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-158">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-158">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[<span data-ttu-id="1064d-160">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-162">Objective-C</span></span>](#tab/objc)
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


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a><span data-ttu-id="1064d-163">Владелец календаря. Обновление разрешений для существующего получателя общего доступа или делегата в календаре</span><span class="sxs-lookup"><span data-stu-id="1064d-163">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>

<span data-ttu-id="1064d-164">С согласия Алекса или администратора вы можете обновить разрешения, назначенные существующему получателю общего доступа или делегату (определяется свойством **role**), если новые разрешения поддерживаются свойством **allowedRoles**, настроенным изначально для получателя общего доступа или делегата для этого календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-164">With the consent of Alex or administrator, you can update the permissions assigned to an existing sharee or delegate (specified by the **role** property), as long as the new permissions are supported by those **allowedRoles** set up initially for the sharee or delegate for that calendar.</span></span> 

<span data-ttu-id="1064d-165">Кроме свойства **role**, вы не можете обновлять другие свойства существующего получателя общего доступа или делегата.</span><span class="sxs-lookup"><span data-stu-id="1064d-165">Aside from the **role** property, you cannot update other properties of an existing sharee or delegate.</span></span> <span data-ttu-id="1064d-166">Изменение значения свойства **emailAddress** требует удаления получателя общего доступа или делегата и повторной настройки нового экземпляра **calendarPermission**.</span><span class="sxs-lookup"><span data-stu-id="1064d-166">Changing the **emailAddress** property value requires deleting the sharee or delegate and setting up a new instance of **calendarPermission** again.</span></span>

<span data-ttu-id="1064d-167">В примере из этого раздела обновляется свойство **role** с изменением разрешения существующего получателя общего доступа Адель с `read` на `write` для пользовательского календаря "Детские праздники".</span><span class="sxs-lookup"><span data-stu-id="1064d-167">The example in this section updates the **role** property, changing the permission of an existing sharee, Adele, from `read` to `write` for the custom calendar "Kids parties".</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-168">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-168">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-169">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `Calendars.ReadWrite` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-169">Use the least privileged delegated or application permission, `Calendars.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-170">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-170">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1064d-172">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-174">Objective-C</span></span>](#tab/objc)
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


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="1064d-175">Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-175">Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="1064d-176">Содержание:</span><span class="sxs-lookup"><span data-stu-id="1064d-176">In this section:</span></span>

- [<span data-ttu-id="1064d-177">Владелец календаря. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-177">Calendar owner: Get properties of a shared or delegated calendar</span></span>](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [<span data-ttu-id="1064d-178">Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-178">Sharee or delegate: Get properties of shared or delegated calendar</span></span>](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

<span data-ttu-id="1064d-179">В этом примере Алекс делегировал свой основной календарь и предоставил делегату Меган Боуен разрешение на просмотр элементов календаря, помеченных как частные.</span><span class="sxs-lookup"><span data-stu-id="1064d-179">Recalling in this example, Alex has delegated his primary calendar and given the delegate, Megan Bowen, the permission to view calendar items that are marked private.</span></span>
<span data-ttu-id="1064d-180">В этом разделе показаны свойства делегированного календаря, сначала с точки зрения и с согласия владельца (Алекс), а затем с точки зрения и с согласия делегата (Меган).</span><span class="sxs-lookup"><span data-stu-id="1064d-180">This section shows the properties of the delegated calendar, first from the perspective of and with the consent of the owner, Alex, and then from the perspective of and with the consent of the delegate, Megan.</span></span> <span data-ttu-id="1064d-181">Согласие администратора также поддерживается для каждого случая.</span><span class="sxs-lookup"><span data-stu-id="1064d-181">Consent from the administrator also works for each case.</span></span>

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="1064d-182">Владелец календаря. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-182">Calendar owner: Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="1064d-183">В примере из этого раздела выполняется получение свойств основного календаря с точки зрения владельца (Алекс).</span><span class="sxs-lookup"><span data-stu-id="1064d-183">The example in this section gets the properties of the primary calendar from the perspective of the owner, Alex.</span></span> 

<span data-ttu-id="1064d-184">Обратите внимание на следующие свойства от имени Алекса:</span><span class="sxs-lookup"><span data-stu-id="1064d-184">Note the following properties on Alex' behalf:</span></span>

- <span data-ttu-id="1064d-185">Свойство **canShare** имеет значение true, так как Алекс является владельцем.</span><span class="sxs-lookup"><span data-stu-id="1064d-185">**canShare** is true as Alex is the owner.</span></span>
- <span data-ttu-id="1064d-186">Свойство **canViewPrivateItems** имеет значение true, так как Алекс является владельцем.</span><span class="sxs-lookup"><span data-stu-id="1064d-186">**canViewPrivateItems** is true since Alex is the owner.</span></span>
- <span data-ttu-id="1064d-187">Свойству **isShared** присвоено значение true, так как Алекс настроил делегата для этого календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-187">**isShared** is set to true, as Alex has set up a delegate for this calendar.</span></span>
- <span data-ttu-id="1064d-188">Свойство **isSharedWithMe** всегда имеет значение false для владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-188">**isSharedWithMe** is always false for the calendar owner.</span></span>
- <span data-ttu-id="1064d-189">Свойство **owner** отображает Алекса в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-189">**owner** shows Alex as the owner.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-190">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-190">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-191">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `Calendars.Read` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-191">Use the least privileged delegated or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-192">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-192">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[<span data-ttu-id="1064d-194">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-196">Objective-C</span></span>](#tab/objc)
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


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a><span data-ttu-id="1064d-197">Получатель общего доступа или делегат. Получение свойств общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-197">Sharee or delegate: Get properties of shared or delegated calendar</span></span>

<span data-ttu-id="1064d-198">В примере из этого раздела выполняется получение свойств того же календаря с точки зрения делегата (Меган).</span><span class="sxs-lookup"><span data-stu-id="1064d-198">The example in this section gets the properties of the same calendar from the perspective of the delegate, Megan.</span></span> 

<span data-ttu-id="1064d-199">Обратите внимание на следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="1064d-199">Note the following properties:</span></span>

- <span data-ttu-id="1064d-200">Свойство **name** календаря по умолчанию соответствует отображаемому имени владельца.</span><span class="sxs-lookup"><span data-stu-id="1064d-200">**name** of the calendar is by default the owner's display name.</span></span> <span data-ttu-id="1064d-201">В этом случае это Alex Wilber (Алекс Уилбер), так как календарь Алекса делегирован Меган.</span><span class="sxs-lookup"><span data-stu-id="1064d-201">In this case, it's "Alex Wilber", since this is Alex' calendar delegated to Megan.</span></span> 
- <span data-ttu-id="1064d-202">Свойство **canShare** имеет значение false, так как Меган не является владельцем этого календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-202">**canShare** is false, since Megan is not the owner of this calendar.</span></span>
- <span data-ttu-id="1064d-203">Свойство **canViewPrivateItems** имеет значение true для делегата Меган, настроенное Алексом.</span><span class="sxs-lookup"><span data-stu-id="1064d-203">**canViewPrivateItems** is true for the delegate Megan, as set up by Alex.</span></span> <span data-ttu-id="1064d-204">Для получателя общего доступа, не являющегося делегатом, это свойство всегда имеет значение false.</span><span class="sxs-lookup"><span data-stu-id="1064d-204">For a sharee that is not a delegate, this property is always false.</span></span>
- <span data-ttu-id="1064d-205">Свойство **isShared** имеет значение false.</span><span class="sxs-lookup"><span data-stu-id="1064d-205">**isShared** is false.</span></span> <span data-ttu-id="1064d-206">Это свойство указывает только для _владельца_ календаря, был ли к календарю предоставлен общий доступ или он был делегирован.</span><span class="sxs-lookup"><span data-stu-id="1064d-206">This property indicates only to a calendar _owner_ whether the calendar has been shared or delegated.</span></span>
- <span data-ttu-id="1064d-207">Свойство **isSharedWithMe** имеет значение true, так как Меган является делегатом.</span><span class="sxs-lookup"><span data-stu-id="1064d-207">**isSharedWithMe** property is true, since Megan is a delegate.</span></span>
- <span data-ttu-id="1064d-208">Свойство **canEdit** имеет значение true, так как делегаты, включая Меган, обладают доступом с разрешением на запись.</span><span class="sxs-lookup"><span data-stu-id="1064d-208">**canEdit** is true, since delegates, including Megan, have write access.</span></span>
- <span data-ttu-id="1064d-209">Свойству **owner** присвоено значение Alex (Алекс).</span><span class="sxs-lookup"><span data-stu-id="1064d-209">**owner** is set to Alex.</span></span>

> [!NOTE] 
> <span data-ttu-id="1064d-210">Получатель общего доступа или делегат может настраивать только свойство **name** общего/делегированного календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-210">A sharee or delegate can customize only the **name** property of a shared/delegated calendar.</span></span> <span data-ttu-id="1064d-211">Изменение отображается только для него самого. Владелец календаря не видит таких изменений имени календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-211">The update is visible only to themselves; the calendar owner does not see such calendar name changes.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-212">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-212">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-213">Для выполнения этой операции воспользуйтесь делегированным разрешением `Calendars.Read.Shared` или разрешением для приложений `Calendars.Read` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-213">Use the least privileged delegated permission, `Calendars.Read.Shared`, or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-214">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-214">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[<span data-ttu-id="1064d-216">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-218">Objective-C</span></span>](#tab/objc)
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


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a><span data-ttu-id="1064d-219">Получение или настройка параметров почтового ящика для получения приглашений на собрания и ответов на них</span><span class="sxs-lookup"><span data-stu-id="1064d-219">Get or set mailbox setting to receive meeting requests and responses</span></span>

<span data-ttu-id="1064d-220">Содержание:</span><span class="sxs-lookup"><span data-stu-id="1064d-220">In this section:</span></span>

- [<span data-ttu-id="1064d-221">Получение параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="1064d-221">Get delegation delivery setting for a user's mailbox</span></span>](#get-delegation-delivery-setting-for-a-users-mailbox)
- [<span data-ttu-id="1064d-222">Настройка параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="1064d-222">Set delegation delivery setting for a user's mailbox</span></span>](#set-delegation-delivery-setting-for-a-users-mailbox)

<span data-ttu-id="1064d-223">В зависимости от уровня делегирования, предпочитаемого владельцем календаря, владелец может указать, кто должен получать приглашения на собрания и ответы на них, чтобы управлять собраниями в календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-223">Depending on the level of delegation a calendar owner prefers, the owner can specify who should receive meeting requests and responses to manage meetings on the calendar.</span></span> 

<span data-ttu-id="1064d-224">Программным способом можно получить или настроить свойство **delegateMeetingMessageDeliveryOptions** объекта [mailboxSettings](/graph/api/resources/mailboxsettings) владельца календаря, чтобы указать, кому Outlook должен направлять экземпляры [eventMessageRequest](/graph/api/resources/eventmessagerequest) и [eventMessageResponse](/graph/api/resources/eventmessageresponse):</span><span class="sxs-lookup"><span data-stu-id="1064d-224">Programmatically, you can get or set the **delegateMeetingMessageDeliveryOptions** property of the calendar owner's [mailboxSettings](/graph/api/resources/mailboxsettings) to specify to whom Outlook should direct [eventMessageRequest](/graph/api/resources/eventmessagerequest) and [eventMessageResponse](/graph/api/resources/eventmessageresponse) instances:</span></span>

- `sendToDelegateOnly`

    <span data-ttu-id="1064d-225">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** только делегатам.</span><span class="sxs-lookup"><span data-stu-id="1064d-225">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to only delegates.</span></span> <span data-ttu-id="1064d-226">Это параметр по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1064d-226">This is the default setting.</span></span> <span data-ttu-id="1064d-227">Владелец может просматривать ответы на приглашения на собрания или отвечать на приглашения с помощью соответствующего объекта **event** в делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-227">The owner can see responses to a meeting or respond to an invitation through the corresponding **event** in the delegated calendar.</span></span>
- `sendToDelegateAndInformationToPrincipal`

    <span data-ttu-id="1064d-228">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря.</span><span class="sxs-lookup"><span data-stu-id="1064d-228">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner.</span></span> <span data-ttu-id="1064d-229">Только делегатам доступны параметры для принятия и отклонения приглашения на собрание. Владельцу отправляется уведомление в виде обычного сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1064d-229">Only the delegates see the option to accept or decline a meeting request, and the notification sent to the owner appears like a normal email message.</span></span> <span data-ttu-id="1064d-230">Владелец может ответить на приглашение, открыв объект **event** в делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="1064d-230">The owner can still respond to the meeting by opening the **event** in the delegated calendar and responding.</span></span>
- `sendToDelegateAndPrincipal`

    <span data-ttu-id="1064d-231">Outlook должен направлять экземпляры **eventMessageRequest** и **eventMessageResponse** делегатам и владельцу календаря, любой из которых может ответить на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="1064d-231">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner, either of whom can respond to the meeting request.</span></span>

<span data-ttu-id="1064d-232">Это параметр на уровне почтового ящика, поэтому этот параметр применяется ко всем делегатам владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1064d-232">This is a mailbox-wide setting, so the same setting applies to all delegates of the mailbox owner.</span></span>

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="1064d-233">Получение параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="1064d-233">Get delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="1064d-234">В примере из этого раздела выполняется получение объекта **mailboxSettings** владельца календаря, который разрешает Outlook направлять приглашения на собрания и ответы на них только делегатам календаря. Таким образом, свойству **delegateMeetingMessageDeliveryOptions** присвоено значение `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="1064d-234">The example in this section gets the **mailboxSettings** of a calendar owner who lets Outlook direct meeting requests and responses to only calendar delegates; that is, **delegateMeetingMessageDeliveryOptions** is set to `sendToDelegateOnly`.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-235">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-235">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-236">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `MailboxSettings.Read` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-236">Use the least privileged delegated or application permission, `MailboxSettings.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-237">Дополнительные сведения о разрешениях, необходимых для работы с почтовыми ящиками, см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-237">For more information about mailbox permissions, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[<span data-ttu-id="1064d-239">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-241">Objective-C</span></span>](#tab/objc)
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

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="1064d-242">Настройка параметра доставки при делегировании для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="1064d-242">Set delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="1064d-243">В примере из этого раздела выполняется обновление свойства **delegateMeetingMessageDeliveryOptions** с присвоением ему значения `sendToDelegateAndPrincipal`, чтобы Outlook направлял приглашения на собрания и ответы на них в делегированном календаре всем делегатам и владельцу.</span><span class="sxs-lookup"><span data-stu-id="1064d-243">The example in this section updates the **delegateMeetingMessageDeliveryOptions** property to `sendToDelegateAndPrincipal`, to have Outlook direct meeting requests and responses of the delegated calendar to all delegates and the owner.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-244">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-244">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-245">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `MailboxSettings.ReadWrite` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-245">Use the least privileged delegated or application permission, `MailboxSettings.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-246">Дополнительные сведения о разрешениях, необходимых для работы с почтовыми ящиками, см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-246">For more information about mailbox permissions, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-247">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1064d-248">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-250">Objective-C</span></span>](#tab/objc)
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


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a><span data-ttu-id="1064d-251">Удаление получателя общего доступа или делегата календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-251">Delete a sharee or delegate of a calendar</span></span>

<span data-ttu-id="1064d-252">В примере ниже Алекс удаляет Меган из роли получателя общего доступа к календарю "Детские праздники".</span><span class="sxs-lookup"><span data-stu-id="1064d-252">In the example below, Alex deletes Megan as a sharee of the "Kids parties" calendar.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="1064d-253">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1064d-253">Microsoft Graph permissions</span></span>
<span data-ttu-id="1064d-254">Для выполнения этой операции воспользуйтесь делегированным разрешением или разрешением для приложений `Calendars.ReadWrite` соответственно.</span><span class="sxs-lookup"><span data-stu-id="1064d-254">Use the least privileged delegated or application permission, `Calendars.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="1064d-255">Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="1064d-255">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="1064d-256">HTTP</span><span class="sxs-lookup"><span data-stu-id="1064d-256">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[<span data-ttu-id="1064d-257">C#</span><span class="sxs-lookup"><span data-stu-id="1064d-257">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1064d-258">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1064d-258">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1064d-259">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1064d-259">Objective-C</span></span>](#tab/objc)
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


## <a name="next-steps"></a><span data-ttu-id="1064d-260">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1064d-260">Next steps</span></span>

<span data-ttu-id="1064d-261">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="1064d-261">Find out more about:</span></span>

- <span data-ttu-id="1064d-262">Как клиенты Outlook поддерживают предоставление общего доступа к календарям и их делегирование:</span><span class="sxs-lookup"><span data-stu-id="1064d-262">How the Outlook clients support sharing and delegating calendars:</span></span>
  - [<span data-ttu-id="1064d-263">Предоставление общего доступа к календарю Outlook другим пользователям</span><span class="sxs-lookup"><span data-stu-id="1064d-263">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [<span data-ttu-id="1064d-264">Предоставление другому пользователю разрешения на управление собственной почтой и календарем в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="1064d-264">Allow someone else to manage your mail and calendar as a delegate</span></span>](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [<span data-ttu-id="1064d-265">Предоставление общего доступа к календарю в Outlook в Интернете</span><span class="sxs-lookup"><span data-stu-id="1064d-265">Share your calendar in Outlook on the web</span></span>](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [<span data-ttu-id="1064d-266">Делегирование доступа к календарю в Outlook в Интернете</span><span class="sxs-lookup"><span data-stu-id="1064d-266">Calendar delegation in Outlook on the web</span></span>](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [<span data-ttu-id="1064d-267">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="1064d-267">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="1064d-268">Создание событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="1064d-268">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="1064d-269">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="1064d-269">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="1064d-270">[API календаря](/graph/api/resources/calendar) в бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1064d-270">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph beta.</span></span>
