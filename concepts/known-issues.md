---
title: Известные проблемы с Microsoft Graph
description: В этой статье описываются известные проблемы, связанные с Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 07ee284f40264c76ec6156235fab651fff77cfe6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777007"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="6cdcf-103">Известные проблемы с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6cdcf-103">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="6cdcf-104">В этой статье описываются известные проблемы, связанные с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-104">This article describes known issues with Microsoft Graph.</span></span> 

<span data-ttu-id="6cdcf-105">Чтобы сообщить об известных проблемах, перейдите на[поддержки Microsoft Graph](https://developer.microsoft.com/graph/support).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-105">To report a known issue, see the [Microsoft Graph support](https://developer.microsoft.com/graph/support) page.</span></span>

<span data-ttu-id="6cdcf-106">Сведения о последних обновлениях API в Microsoft Graph см. в [журнале изменений Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-106">For information about the latest updates to the Microsoft Graph API, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="bookings"></a><span data-ttu-id="6cdcf-107">Bookings</span><span class="sxs-lookup"><span data-stu-id="6cdcf-107">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="6cdcf-108">Ошибка ErrorExceededFindCountLimit при запросе bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="6cdcf-108">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="6cdcf-109">При получении списка по запросу `bookingBusinesses` возвращается ошибка с указанным ниже кодом, если у организации есть несколько компаний в Bookings, а учетная запись, с использованием которой отправлен запрос, не принадлежит администратору.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-109">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="6cdcf-110">В качестве обходного решения можно ограничить группу компаний, возвращаемых по запросу, указав параметр `query`. Пример:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-110">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a><span data-ttu-id="6cdcf-111">Календари</span><span class="sxs-lookup"><span data-stu-id="6cdcf-111">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="6cdcf-112">Доступ к общему календарю</span><span class="sxs-lookup"><span data-stu-id="6cdcf-112">Accessing a shared calendar</span></span>

<span data-ttu-id="6cdcf-113">При использовании следующей операции для доступа к событиям в календаре другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-113">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET /users/{id}/calendars/{id}/events
```

<span data-ttu-id="6cdcf-p101">Может возникнуть ошибка HTTP 500 `ErrorInternalServerTransientError`. Ошибка возникает, потому что:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p101">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="6cdcf-116">Существуют два способа реализации общего доступа к календарю, которые для ясности мы будем называть "старый" способ и "новый" способ.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-116">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="6cdcf-117">Новый способ в настоящее время доступен для предоставления доступа к календарям с разрешениями на просмотр или редактирование, но не с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-117">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="6cdcf-118">С помощью REST API календаря можно просматривать и редактировать общие календари, только если доступ к ним предоставлен **новым** способом.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-118">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="6cdcf-119">С помощью REST API календаря нельзя просматривать или редактировать общие календари (или их события), если доступ к ним предоставлен **старым** способом.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-119">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="6cdcf-120">Если доступ к календарю был предоставлен с разрешениями на просмотр или редактирование, но старым способом, вы можете вручную обновить календарь, чтобы использовать новый способ.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-120">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="6cdcf-121">Чтобы можно было использовать новый способ, со временем Outlook автоматически обновит все общие календари, в том числе те, доступ к которым предоставлен с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-121">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="6cdcf-122">Чтобы с этой целью вручную обновить общий календарь, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-122">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="6cdcf-123">Получатель удаляет календарь, доступ к которому был ранее ему предоставлен.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-123">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="6cdcf-124">Владелец повторно предоставляет доступ к календарю в Outlook в Интернете, Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-124">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="6cdcf-p103">Получатель повторно принимает календарь, используя Outlook в Интернете. (Скоро можно будет использовать другие клиенты Outlook.)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p103">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="6cdcf-127">Доступ к календарю успешно предоставлен новым способом, если получатель может просмотреть его в Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-127">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="6cdcf-p104">Календарь, доступ к которому предоставлен новым способом, выглядит как один из стандартных календарей в вашем почтовом ящике. С помощью REST API календаря можно просматривать и редактировать события в общем календаре, как в своем собственном. Например:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p104">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="6cdcf-131">Добавление календарей ICS в почтовый ящик пользователя и доступ к ним</span><span class="sxs-lookup"><span data-stu-id="6cdcf-131">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="6cdcf-132">В настоящее время календари ICS поддерживаются частично:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-132">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="6cdcf-133">Вы можете добавить календарь ICS в почтовый ящик пользователя через интерфейс пользователя, но не через API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-133">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="6cdcf-p105">[Перечисление календарей пользователя](/graph/api/user-list-calendars) позволяет получить свойства **name**, **color** и **id** всех [календарей](/graph/api/resources/calendar) в группе календарей пользователя по умолчанию или указанной группе календарей, в том числе календарей ICS. URL-адрес ICS невозможно хранить и открывать в ресурсе calendar.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p105">[Listing the user's calendars](/graph/api/user-list-calendars) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="6cdcf-136">Вы также можете [отобразить события](/graph/api/calendar-list-events) календаря ICS.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-136">You can also [list the events](/graph/api/calendar-list-events) of an ICS-based calendar.</span></span>

### <a name="attaching-large-files-to-events"></a><span data-ttu-id="6cdcf-137">Прикрепление больших файлов к событиям</span><span class="sxs-lookup"><span data-stu-id="6cdcf-137">Attaching large files to events</span></span>
<span data-ttu-id="6cdcf-138">Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-138">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="6cdcf-139">С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-139">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="6cdcf-140">Поддержка свойства onlineMeetingUrl для Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6cdcf-140">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="6cdcf-141">В настоящее время свойство **onlineMeetingUrl** ресурса [event](/graph/api/resources/event) для собрания Skype означает URL-адрес для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-141">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event) would indicate the online meeting URL.</span></span> <span data-ttu-id="6cdcf-142">Однако для ресурса event собрания в Microsoft Teams задано значение NULL.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-142">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

<span data-ttu-id="6cdcf-143">В бета-версии предлагается обходное решение, позволяющее использовать свойство **onlineMeetingProvider** ресурса [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) с целью убедиться, что поставщиком является Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-143">The beta version offers a workaround, where you can use the **onlineMeetingProvider** property of an [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) to verify if the provider is Microsoft Teams.</span></span> <span data-ttu-id="6cdcf-144">С помощью свойства **onlineMeeting** ресурса **event** вы можете получить доступ к объекту **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-144">Through the **onlineMeeting** property of the **event**, you can access the **joinUrl**.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="6cdcf-145">Уведомления об изменениях</span><span class="sxs-lookup"><span data-stu-id="6cdcf-145">Change notifications</span></span>

### <a name="additional-notifications-for-users"></a><span data-ttu-id="6cdcf-146">Дополнительные уведомления для пользователей</span><span class="sxs-lookup"><span data-stu-id="6cdcf-146">Additional notifications for users</span></span>

<span data-ttu-id="6cdcf-147">[Подписки](/graph/api/resources/subscription) на изменения для **пользователя** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании пользователя и обратимом удалении пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-147">[Subscriptions](/graph/api/resources/subscription) to changes for **user** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on user creation and user soft deletion.</span></span>

### <a name="additional-notifications-for-groups"></a><span data-ttu-id="6cdcf-148">Дополнительные уведомления для групп</span><span class="sxs-lookup"><span data-stu-id="6cdcf-148">Additional notifications for groups</span></span>

<span data-ttu-id="6cdcf-149">[Подписки](/graph/api/resources/subscription) на изменения для **группы** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании группы и обратимом удалении группы.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-149">[Subscriptions](/graph/api/resources/subscription) to changes for **group** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on group creation and group soft deletion.</span></span>

## <a name="cloud-communications"></a><span data-ttu-id="6cdcf-150">Облачные коммуникации</span><span class="sxs-lookup"><span data-stu-id="6cdcf-150">Cloud communications</span></span> 

<span data-ttu-id="6cdcf-151">Клиент Microsoft Teams не отображает меню **Просмотреть сведения о собрании** для собраний канала, созданных с помощью API коммуникаций из облака.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-151">The Microsoft Teams client does not show the **View Meeting details**  menu for channel meetings created via the cloud communications API.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="6cdcf-152">Приложения Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="6cdcf-152">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="6cdcf-153">Приложения CSP должны использовать конечную точку Azure AD</span><span class="sxs-lookup"><span data-stu-id="6cdcf-153">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="6cdcf-p109">Приложения CSP должны получать маркеры из конечных точек Azure AD (версии 1) для успешного вызова Microsoft Graph в своих клиентах, управляемых партнерами. В настоящее время получение маркера через конечную точку Azure AD версии 2.0 не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p109">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="6cdcf-156">В некоторых клиентах предоставленные приложениям CSP разрешения не работают</span><span class="sxs-lookup"><span data-stu-id="6cdcf-156">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="6cdcf-157">Предоставленные приложениям CSP разрешения могут не работать в некоторых клиентах.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-157">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="6cdcf-158">После первого входа в приложение, использующее делегированные разрешения, в новом клиенте может возникнуть эта ошибка: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-158">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="6cdcf-159">Приложение, использующее разрешения для приложений, может получить маркер, но ему может быть неожиданно отказано в доступе при вызове Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-159">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="6cdcf-160">Мы делаем все возможное, чтобы как можно быстрее исправить эту ошибку.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-160">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="6cdcf-161">Для целей разработки и тестирования можно использовать следующее временное решение.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-161">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="6cdcf-p110">**ПРИМЕЧАНИЕ.** Это не окончательное решение и предназначено только для целей разработки.  Оно станет ненужным после исправления упомянутой выше ошибки.  Удалять указанный ниже субъект-службу не нужно.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p110">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="6cdcf-p111">Откройте сеанс Azure AD PowerShell 2 и подключитесь к клиенту `customer`, введя учетные данные администратора в окне входа. Скачать и установить Azure AD PowerShell 2 можно [здесь](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p111">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="6cdcf-167">Создайте субъект-службу Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-167">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a><span data-ttu-id="6cdcf-168">Контакты</span><span class="sxs-lookup"><span data-stu-id="6cdcf-168">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="6cdcf-169">Контакты организации доступны только в бета-версии</span><span class="sxs-lookup"><span data-stu-id="6cdcf-169">Organization contacts available in only beta</span></span>

<span data-ttu-id="6cdcf-p112">В настоящее время поддерживаются только личные контакты. В настоящее время контакты организации не поддерживаются в версии `/v1.0`, но их можно найти в версии `/beta`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p112">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="6cdcf-172">Папка контактов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6cdcf-172">Default contacts folder</span></span>

<span data-ttu-id="6cdcf-173">В версии `/v1.0` запрос `GET /me/contactFolders` не включает папку контактов пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-173">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="6cdcf-p113">Эта ошибка будет исправлена. Чтобы получить идентификатор папки контактов по умолчанию, вы можете использовать следующий запрос на [отображение контактов](/graph/api/user-list-contacts) и свойство **parentFolderId**:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p113">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="6cdcf-176">В указанном выше запросе:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-176">In the above query:</span></span>

1. <span data-ttu-id="6cdcf-177">`/me/contacts?$top=1` возвращает свойства [контакта](/graph/api/resources/contact) в папке контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-177">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="6cdcf-178">При добавлении `&$select=parentFolderId` возвращается только свойство контакта **parentFolderId** — идентификатор папки контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-178">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="6cdcf-179">Доступ к контактам через папку контактов в бета-версии</span><span class="sxs-lookup"><span data-stu-id="6cdcf-179">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="6cdcf-180">В настоящее время в версии `/beta` существует проблема, из-за которой нельзя получить доступ к ресурсу [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true), указав его родительскую папку в URL-адресе запроса REST, как показано в 2 приведенных ниже сценариях.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-180">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="6cdcf-181">Доступ к контакту из папки верхнего уровня [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-181">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="6cdcf-p114">Доступ к контакту в дочерней папке папки **contactFolder**.  В приведенном ниже примере показан один уровень вложения, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p114">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="6cdcf-184">Кроме того, вы можете просто [получить](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) контакт по его идентификатору, как показано ниже, так как конечная точка /contacts для запроса GET в версии `/beta` применяется ко всем контактам в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-184">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a><span data-ttu-id="6cdcf-185">Разностный запрос</span><span class="sxs-lookup"><span data-stu-id="6cdcf-185">Delta query</span></span>

* <span data-ttu-id="6cdcf-186">При отслеживании изменений в отношениях иногда неправильно возвращается контекст OData.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-186">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="6cdcf-187">Расширения схемы (устаревшие) не возвращаются с оператором $select и возвращаются без него.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-187">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="6cdcf-188">Клиенты не могут отслеживать изменения в открытых расширениях и зарегистрированных расширениях схемы.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-188">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="extensions"></a><span data-ttu-id="6cdcf-189">Расширения</span><span class="sxs-lookup"><span data-stu-id="6cdcf-189">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="6cdcf-190">Отслеживание изменений не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6cdcf-190">Change tracking is not supported</span></span>

<span data-ttu-id="6cdcf-191">Отслеживание изменений не поддерживается для свойств открытых расширений и расширений схемы.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-191">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="6cdcf-192">Одновременное создание ресурса и открытого расширения</span><span class="sxs-lookup"><span data-stu-id="6cdcf-192">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="6cdcf-p115">Невозможно указать открытое расширение при создании экземпляра **administrativeUnit**, **device**, **group**, **organization** или **user**. Сначала необходимо создать экземпляр, а затем указать данные открытого расширения в последующем запросе ``POST`` к этому экземпляру.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p115">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="6cdcf-195">Создание экземпляра ресурса с одновременным добавлением данных расширения схемы</span><span class="sxs-lookup"><span data-stu-id="6cdcf-195">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="6cdcf-196">Вы не можете указать расширение схемы в той же операции, которая создает экземпляр **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-196">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="6cdcf-197">Сперва нужно создать экземпляр ресурса, а затем выполнить операцию `PATCH` для этого экземпляра, чтобы добавить расширение схемы и пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-197">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="6cdcf-198">Для каждого экземпляра ресурса разрешено не более 100 значений свойства расширения схемы</span><span class="sxs-lookup"><span data-stu-id="6cdcf-198">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="6cdcf-199">В настоящее время для каждого экземпляра таких ресурсов каталога, как **device**, **group** и **user**, можно установить не более 100 значений свойства расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-199">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a><span data-ttu-id="6cdcf-200">Обновление определения schemaExtension с помощью проводника Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6cdcf-200">Updating a schemaExtension definition using Microsoft Graph Explorer</span></span>

<span data-ttu-id="6cdcf-201">При использовании `PATCH` для обновления schemaExtension с помощью проводника Graph необходимо указать свойство **owner** и задать для него текущее значение `appid` (которое должно быть `appId` имеющегося приложения).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-201">When using `PATCH` to update a schemaExtension using Graph Explorer, you must specify the **owner** property and set it to its current `appid` value (which will need to be an `appId` of an application that you own).</span></span> <span data-ttu-id="6cdcf-202">Это также относится к любому клиентскому приложению, у которого `appId` отличается от **owner**.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-202">This is also the case for any client application whose `appId` is not the same as the **owner**.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="6cdcf-203">Фильтрация по свойствам расширения схемы поддерживается не для всех типов объектов</span><span class="sxs-lookup"><span data-stu-id="6cdcf-203">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="6cdcf-204">Фильтрация по свойствам расширения схемы (с помощью выражения `$filter`) не поддерживается для типов объектов Outlook **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-204">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="files-onedrive"></a><span data-ttu-id="6cdcf-205">Файлы (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-205">Files (OneDrive)</span></span>

* <span data-ttu-id="6cdcf-206">При первом доступе к личному диску пользователя с помощью Microsoft Graph до открытия им своего личного сайта в браузере возвращается ответ 401.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-206">First time access to a user's personal drive through Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="groups"></a><span data-ttu-id="6cdcf-207">Группы</span><span class="sxs-lookup"><span data-stu-id="6cdcf-207">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="6cdcf-208">Разрешения для групп и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6cdcf-208">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="6cdcf-209">Microsoft Graph предоставляет два разрешения ([*Group.Read.All*](permissions-reference.md#group-permissions) и [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) для доступа к API для групп и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-209">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="6cdcf-210">Эти разрешения должен предоставить администратор.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-210">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="6cdcf-211">В будущем мы планируем добавить новые разрешения для групп и команд, которые смогут предоставлять пользователи.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-211">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="6cdcf-p119">Кроме того, только API для базового администрирования групп и управления ими поддерживает доступ с помощью разрешений только для приложений или делегированных разрешений. Все остальные функции API групп поддерживают только делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p119">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="6cdcf-214">Примеры функций групп, поддерживающих разрешения только для приложений и делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-214">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="6cdcf-215">создание и удаление групп;</span><span class="sxs-lookup"><span data-stu-id="6cdcf-215">Creating and deleting groups</span></span>
* <span data-ttu-id="6cdcf-216">получение и обновление свойств групп, связанных с администрированием групп и управлением ими;</span><span class="sxs-lookup"><span data-stu-id="6cdcf-216">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="6cdcf-217">синхронизация, типы и [параметры каталогов](/graph/api/resources/directoryobject) групп;</span><span class="sxs-lookup"><span data-stu-id="6cdcf-217">Group [directory settings](/graph/api/resources/directoryobject), type, and synchronization</span></span>
* <span data-ttu-id="6cdcf-218">владельцы и члены групп.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-218">Group owners and membership</span></span>
* <span data-ttu-id="6cdcf-219">Получение групповых бесед</span><span class="sxs-lookup"><span data-stu-id="6cdcf-219">Getting group conversations and threads</span></span>

<span data-ttu-id="6cdcf-220">Примеры функций групп, поддерживающих только делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-220">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="6cdcf-221">Групповые события, фотографии</span><span class="sxs-lookup"><span data-stu-id="6cdcf-221">Group events, photo</span></span>
* <span data-ttu-id="6cdcf-222">внешние отправители, разрешенные или запрещенные отправители, подписка на группы;</span><span class="sxs-lookup"><span data-stu-id="6cdcf-222">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="6cdcf-223">избранное пользователей и счетчик непросмотренных элементов.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-223">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="6cdcf-224">Политика</span><span class="sxs-lookup"><span data-stu-id="6cdcf-224">Policy</span></span>

<span data-ttu-id="6cdcf-225">Использование Microsoft Graph для создания группы Microsoft 365 и присвоения ей имени в обход всех групповых политик Microsoft 365, настроенных через Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-225">Using Microsoft Graph to create and name a Microsoft 365 group bypasses any Microsoft 365 group policies that are configured through Outlook on the web.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="6cdcf-226">Установка свойства allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="6cdcf-226">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="6cdcf-227">В настоящее время существует проблема, из-за которой невозможно установить свойство **allowExternalSenders** группы в операции POST или PATCH как в `/v1.0`, так и в `/beta`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-227">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="6cdcf-228">Работа с запросами изменений</span><span class="sxs-lookup"><span data-stu-id="6cdcf-228">Using delta query</span></span>

<span data-ttu-id="6cdcf-229">Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-229">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="identity-and-access--application-and-service-principal-apis"></a><span data-ttu-id="6cdcf-230">Удостоверение и доступ | API приложений и субъектов-служб</span><span class="sxs-lookup"><span data-stu-id="6cdcf-230">Identity and access | Application and service principal APIs</span></span>

<span data-ttu-id="6cdcf-p120">Скоро в объекты [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) будут внесены изменения. Ниже приведено краткое описание текущих ограничений и возможностей API, находящихся в разработке.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p120">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="6cdcf-233">Текущие ограничения:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-233">Current limitations:</span></span>

* <span data-ttu-id="6cdcf-234">Некоторые свойства application (такие как appRoles и addIns) будут доступны только после внесения всех изменений.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-234">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="6cdcf-235">Регистрировать можно только мультитенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-235">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="6cdcf-236">Обновлять можно только приложения, зарегистрированные после первоначального обновления бета-версии.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-236">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="6cdcf-237">Пользователи Azure Active Directory могут регистрировать приложения и добавлять владельцев.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-237">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="6cdcf-238">Поддержка протоколов OpenID Connect и OAuth.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-238">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="6cdcf-239">Невозможно назначение политик приложению.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-239">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="6cdcf-240">Не выполняются операции с ownedObjects, для которых требуется код appId (например, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-240">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="6cdcf-241">В разработке:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-241">In development:</span></span>

* <span data-ttu-id="6cdcf-242">Возможность регистрировать однотенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-242">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="6cdcf-243">Обновления объекта servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-243">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="6cdcf-244">Перевод существующих приложений Azure AD на обновленную модель.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-244">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="6cdcf-245">Поддержка appRoles, предварительно авторизованные клиенты, необязательные утверждения, утверждения членства в группе и брендинг.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-245">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="6cdcf-246">Пользователи учетной записи Майкрософт (MSA) могут регистрировать приложения.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-246">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="6cdcf-247">Поддержка протоколов SAML и WsFed.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-247">Support for SAML and WsFed protocols.</span></span>

## <a name="identity-and-access--conditional-access"></a><span data-ttu-id="6cdcf-248">Удостоверение и доступ | Условный доступ</span><span class="sxs-lookup"><span data-stu-id="6cdcf-248">Identity and access | Conditional access</span></span>

### <a name="permissions"></a><span data-ttu-id="6cdcf-249">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cdcf-249">Permissions</span></span>

<span data-ttu-id="6cdcf-250">В настоящее время для вызова API POST и PATCH требуется разрешение Policy.Read.All.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-250">Currently, the Policy.Read.All permission is required to call POST and PATCH APIs.</span></span> <span data-ttu-id="6cdcf-251">В дальнейшем разрешение Policy.ReadWrite.ConditionalAccess позволит читать политики из каталога.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-251">In the future, the Policy.ReadWrite.ConditionalAccess permission will enable you to read policies from the directory.</span></span>

## <a name="json-batching"></a><span data-ttu-id="6cdcf-252">Пакетная обработка JSON</span><span class="sxs-lookup"><span data-stu-id="6cdcf-252">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="6cdcf-253">Не поддерживаются вложенные пакеты</span><span class="sxs-lookup"><span data-stu-id="6cdcf-253">No nested batch</span></span>

<span data-ttu-id="6cdcf-254">Пакетные запросы JSON не должны содержать вложенных пакетных запросов.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-254">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="6cdcf-255">Все отдельные запросы должны быть синхронными</span><span class="sxs-lookup"><span data-stu-id="6cdcf-255">All individual requests must be synchronous</span></span>

<span data-ttu-id="6cdcf-p122">Все запросы, содержащиеся в пакетном запросе, должны выполняться синхронно. Параметр `respond-async`, если он имеется, будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p122">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="6cdcf-258">Не поддерживается диалоговая обработка</span><span class="sxs-lookup"><span data-stu-id="6cdcf-258">No transactions</span></span>

<span data-ttu-id="6cdcf-p123">В настоящее время Microsoft Graph не поддерживает диалоговую обработку отдельных запросов. Свойство `atomicityGroup` отдельных запросов будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p123">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="6cdcf-261">URI должны быть относительными</span><span class="sxs-lookup"><span data-stu-id="6cdcf-261">URIs must be relative</span></span>

<span data-ttu-id="6cdcf-p124">Всегда указывайте относительные URI в пакетных запросах. Microsoft Graph сделает эти URL-адреса абсолютными с помощью конечной точки версии, включенной в URL-адрес пакета.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p124">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="6cdcf-264">Ограничение на размер пакета</span><span class="sxs-lookup"><span data-stu-id="6cdcf-264">Limit on batch size</span></span>

<span data-ttu-id="6cdcf-265">В настоящее время в пакетный запрос JSON можно включить не более 20 отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-265">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="6cdcf-266">Упрощенные зависимости</span><span class="sxs-lookup"><span data-stu-id="6cdcf-266">Simplified dependencies</span></span>

<span data-ttu-id="6cdcf-p125">Отдельные запросы могут зависеть от других отдельных запросов. В настоящее время запросы могут зависеть только от одного другого запроса и должны соответствовать одному из этих шаблонов:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p125">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="6cdcf-269">Параллельный — для отдельных запросов не указаны зависимости в свойстве `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-269">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="6cdcf-270">Последовательный — все отдельные запросы зависят от предыдущего отдельного запроса.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-270">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="6cdcf-271">Идентичный — для всех отдельных запросов в свойстве `dependsOn` указана одна и та же зависимость.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-271">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="6cdcf-272">После усовершенствования пакетной обработки JSON эти ограничения будут удалены.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-272">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="mail-outlook"></a><span data-ttu-id="6cdcf-273">Почта (Outlook)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-273">Mail (Outlook)</span></span>

### <a name="attaching-large-files-to-messages"></a><span data-ttu-id="6cdcf-274">Вложение больших файлов в сообщения</span><span class="sxs-lookup"><span data-stu-id="6cdcf-274">Attaching large files to messages</span></span>
<span data-ttu-id="6cdcf-275">Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-275">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="6cdcf-276">С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-276">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="6cdcf-277">Параметр comment для создания черновика</span><span class="sxs-lookup"><span data-stu-id="6cdcf-277">The comment parameter for creating a draft</span></span>

<span data-ttu-id="6cdcf-278">Параметр **comment** для создания ответа или черновика ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) не включается в текст полученного черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-278">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="6cdcf-279">При использовании запроса GET для сообщений возвращаются также чаты в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6cdcf-279">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="6cdcf-280">В конечных точках версии 1 и бета-версии данные отклика для `GET /users/id/messages` включают чаты Microsoft Teams, не входящие в область группы или канала.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-280">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="6cdcf-281">Тема этих сообщений чата: "IM".</span><span class="sxs-lookup"><span data-stu-id="6cdcf-281">These chat messages have "IM" as their subject.</span></span>

## <a name="teamwork-microsoft-teams"></a><span data-ttu-id="6cdcf-282">Работа в команде (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-282">Teamwork (Microsoft Teams)</span></span>

### <a name="get-teams-is-not-supported"></a><span data-ttu-id="6cdcf-283">GET / команды не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6cdcf-283">GET /teams is not supported</span></span>

<span data-ttu-id="6cdcf-284">Чтобы получить список команд, см. [список всех команд](teams-list-all-teams.md) и [список ваших команд](/graph/api/user-list-joinedteams).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-284">To get a list of teams, see [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams).</span></span>

### <a name="unable-to-filter-team-members-by-roles"></a><span data-ttu-id="6cdcf-285">Не удается отфильтровать участников команды по ролям</span><span class="sxs-lookup"><span data-stu-id="6cdcf-285">Unable to filter team members by roles</span></span>
<span data-ttu-id="6cdcf-286">Запрос фильтра на получение участников команды на основе их ролей `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')` может не работать.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-286">The filter query to get members of a team based on their roles `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')` might not work.</span></span> <span data-ttu-id="6cdcf-287">Сервер может вернуть `BAD REQUEST`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-287">The server might respond with a `BAD REQUEST`.</span></span>

### <a name="missing-properties-for-chat-members"></a><span data-ttu-id="6cdcf-288">Отсутствующие свойства для участников чатов</span><span class="sxs-lookup"><span data-stu-id="6cdcf-288">Missing properties for chat members</span></span>
<span data-ttu-id="6cdcf-289">В некоторых случаях свойство `tenantId` / `email` / `displayName` для отдельных участников чата может не заполняться в запросах `GET /chats/chat-id/members` или `GET /chats/chat-id/members/membership-id`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-289">In certain instances, the `tenantId` / `email` / `displayName` property for the individual members of a chat might not be populated on a `GET /chats/chat-id/members` or `GET /chats/chat-id/members/membership-id` request.</span></span>

## <a name="users"></a><span data-ttu-id="6cdcf-290">Пользователи</span><span class="sxs-lookup"><span data-stu-id="6cdcf-290">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="6cdcf-291">Нет мгновенного доступа после создания</span><span class="sxs-lookup"><span data-stu-id="6cdcf-291">No instant access after creation</span></span>

<span data-ttu-id="6cdcf-292">Пользователей можно создавать мгновенно с помощью метода POST для объекта user.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-292">Users can be created immediately through a POST on the user entity.</span></span> <span data-ttu-id="6cdcf-293">Для доступа к службам Microsoft 365 пользователю нужна соответствующая лицензия.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-293">A Microsoft 365 license must first be assigned to a user, in order to get access to Microsoft 365 services.</span></span> <span data-ttu-id="6cdcf-294">Из-за распределенного характера службы файлы, сообщения и события этого пользователя станут доступны посредством API Microsoft Graph через 15 минут после назначения лицензии.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-294">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span></span> <span data-ttu-id="6cdcf-295">В течение этого времени приложения будут получать ошибку HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-295">During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="6cdcf-296">Ограничения для фотографий</span><span class="sxs-lookup"><span data-stu-id="6cdcf-296">Photo restrictions</span></span>

<span data-ttu-id="6cdcf-297">Просмотреть и обновить фотографию профиля пользователя можно, только если у пользователя есть почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-297">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span></span> <span data-ttu-id="6cdcf-298">Кроме того, все фотографии, которые *могли* быть сохранены ранее с помощью свойства **thumbnailPhoto** (с помощью Azure AD Graph или службы синхронизации AD Connect), больше не доступны через свойство **photo** Microsoft Graph ресурса [user](/graph/api/resources/user).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-298">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Azure AD Graph or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user) resource.</span></span>
<span data-ttu-id="6cdcf-299">В этом случае, если фотографию не удастся просмотреть или обновить, возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-299">Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a><span data-ttu-id="6cdcf-300">Запрос изменений</span><span class="sxs-lookup"><span data-stu-id="6cdcf-300">Using delta query</span></span>

<span data-ttu-id="6cdcf-301">Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-301">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="6cdcf-302">Отзыв сеансов входа возвращает неправильный код HTTP</span><span class="sxs-lookup"><span data-stu-id="6cdcf-302">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="6cdcf-303">[user: revokeSignInSessions API](/graph/api/user-revokesigninsessions) должен возвращать ответ `204 No content` в случае успешного отзыва и код ошибки HTTP (4xx или 5xx), если запрос не выполнен.  </span><span class="sxs-lookup"><span data-stu-id="6cdcf-303">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="6cdcf-304">Однако из-за проблемы со службой этот API возвращает `200 OK` и логический параметр, который всегда правильный.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-304">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="6cdcf-305">Пока проблема не будет устранена, разработчикам рекомендуется просто интерпретировать код возврата 2xx как успешное выполнение запроса к этому API.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-305">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

### <a name="incomplete-objects-when-using-getbyids-request"></a><span data-ttu-id="6cdcf-306">Неполные объекты при использовании запроса getByIds</span><span class="sxs-lookup"><span data-stu-id="6cdcf-306">Incomplete objects when using getByIds request</span></span>

<span data-ttu-id="6cdcf-307">При запросе объектов с помощью [получения объектов каталога из списка идентификаторов](/graph/api/directoryobject-getbyids) должны возвращаться полные объекты.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-307">Requesting objects using [Get directory objects from a list of IDs](/graph/api/directoryobject-getbyids) should return full objects.</span></span> <span data-ttu-id="6cdcf-308">Однако в настоящее время объекты [user](/graph/api/resources/user) в конечной точке версии 1.0 возвращаются с ограниченным набором свойств.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-308">However, currently [user](/graph/api/resources/user) objects on the v1.0 endpoint are returned with a limited set of properties.</span></span> <span data-ttu-id="6cdcf-309">Временное решение: возврат более полных объектов [user](/graph/api/resources/user) обеспечивается при использовании операции в сочетании с параметром запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-309">As a temporary workaround, when you use the operation in combination with the `$select` query option, more complete [user](/graph/api/resources/user) objects will be returned.</span></span> <span data-ttu-id="6cdcf-310">Это поведение не соответствует спецификациям OData.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-310">This behavior is not in accordance with the OData specifications.</span></span> <span data-ttu-id="6cdcf-311">Так как это поведение может быть изменено в будущем, используйте это временное решение только при указании в параметре `$select=` всех нужных свойств и только если допускается внесение существенных изменений в это временное решение.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-311">Because this behavior might be updated in the future, use this workaround only when you provide `$select=` with all the properties you are interested in, and only if future breaking changes to this workaround are acceptable.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="6cdcf-312">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="6cdcf-312">Query parameter limitations</span></span>

* <span data-ttu-id="6cdcf-313">Не поддерживается несколько пространств имен.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-313">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="6cdcf-314">Не поддерживаются запросы GET для `$ref` и приведение для пользователей, групп, устройств, субъектов-служб и приложений.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-314">GETs on `$ref` and casting are not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="6cdcf-p133">Не поддерживается `@odata.bind`. Это значит, что разработчики не смогут правильно настроить свойство **acceptedSenders** или **rejectedSenders** для группы.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p133">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="6cdcf-317">Отсутствует `@odata.id` для навигации по объектам без вложений (например, сообщениям) при использовании минимальных метаданных.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-317">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="6cdcf-318">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-318">`$expand`:</span></span>
  * <span data-ttu-id="6cdcf-319">Отсутствует поддержка `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-319">No support for `nextLink`</span></span>
  * <span data-ttu-id="6cdcf-320">Поддерживается не более одного уровня развертывания.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-320">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="6cdcf-321">Не поддерживаются дополнительные параметры (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-321">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="6cdcf-322">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-322">`$filter`:</span></span>
  * <span data-ttu-id="6cdcf-323">Конечная точка `/attachments` не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-323">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="6cdcf-324">При ее наличии параметр `$filter` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-324">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="6cdcf-325">Фильтрация нескольких рабочих нагрузок не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-325">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="6cdcf-326">`$search`:</span><span class="sxs-lookup"><span data-stu-id="6cdcf-326">`$search`:</span></span>
  * <span data-ttu-id="6cdcf-327">Полнотекстовый поиск доступен только для некоторых объектов, например сообщений.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-327">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="6cdcf-328">Поиск по нескольким рабочим нагрузкам не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-328">Cross-workload searching is not supported.</span></span>


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="6cdcf-329">Функции, доступные только в REST API Office 365 или API Graph Azure AD</span><span class="sxs-lookup"><span data-stu-id="6cdcf-329">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="6cdcf-330">Некоторые функции еще не доступны в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-330">Some functionality is not yet available in Microsoft Graph.</span></span> <span data-ttu-id="6cdcf-331">Если вы не нашли нужную функцию, можете использовать специальные [REST API Office 365](/previous-versions/office/office-365-api/).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-331">If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](/previous-versions/office/office-365-api/).</span></span> <span data-ttu-id="6cdcf-332">Сведения об Azure Active Directory см. в статье [Миграция приложений Azure AD Graph в Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-332">For Azure Active Directory, see [Migrate Azure AD Graph apps to Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span></span>
