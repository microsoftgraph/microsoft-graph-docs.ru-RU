---
title: Ограничение области разрешений для приложений с указанием определенных почтовых ящиков Exchange Online
description: Чтобы ограничить область разрешений для приложений с указанием определенных почтовых ящиков Exchange Online, потребуется создать политики доступа приложений.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: f31f7bfc8ff72c8f3cb9e6f61185187f50bab7fc
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266838"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="406f3-103">Ограничение области разрешений для приложений с указанием определенных почтовых ящиков Exchange Online</span><span class="sxs-lookup"><span data-stu-id="406f3-103">Scoping application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="406f3-104">Некоторые приложения вызывают Microsoft Graph от своего имени, а не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="406f3-104">Some apps call Microsoft Graph using their own identity and not on behalf of a user.</span></span> <span data-ttu-id="406f3-105">Обычно это фоновые службы и управляющие программы, которые работают на сервере без выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="406f3-105">These are usually background services or daemon apps that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="406f3-106">В таких приложениях используется [поток предоставления учетных данных клиента OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow), обеспечивающий проверку подлинности, и заданы настройки разрешений для приложений, которые позволяют таким приложениям получать доступ ко всем почтовым ящикам организации на сервере Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="406f3-106">These apps make use of [OAuth 2.0 client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which enable such apps to access all mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="406f3-107">Например с помощью разрешения для приложения Mail.Read приложения могут считывать почту во всех почтовых ящиках без выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="406f3-107">For example, the Mail.Read application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="406f3-108">Администраторам, которые хотят ограничить доступ приложения к определенному набору почтовых ящиков, можно воспользоваться командлетом PowerShell **New-ApplicationAccessPolicy**, чтобы настроить управление доступом.</span><span class="sxs-lookup"><span data-stu-id="406f3-108">Administrators who want to limit the app access to a specific set of mailboxes can use the **New-ApplicationAccessPolicy** PowerShell cmdlet to configure access control.</span></span> <span data-ttu-id="406f3-109">В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="406f3-109">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="406f3-110">Эти инструкции относятся к ресурсам Exchange Online и не относятся к другим рабочим нагрузкам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="406f3-110">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="406f3-111">Настройка ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-111">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="406f3-112">Чтобы настроить политику доступа приложения и ограничить область разрешений для приложения, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="406f3-112">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="406f3-113">Подключитесь к Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="406f3-113">Connect to Exchange Online PowerShell.</span></span> <span data-ttu-id="406f3-114">Подробнее см. статью [Подключение к Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="406f3-114">For details, see [Connect to Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2.  <span data-ttu-id="406f3-115">Определите идентификатор клиента приложения и группу безопасности с поддержкой электронной почты, чтобы ограничить доступ приложения.</span><span class="sxs-lookup"><span data-stu-id="406f3-115">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="406f3-116">Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="406f3-116">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="406f3-117">Создайте новую группу безопасности с поддержкой электронной почты или используйте существующую и определите адрес электронной почты для группы.</span><span class="sxs-lookup"><span data-stu-id="406f3-117">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="406f3-118">Создайте политику доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="406f3-118">Create an application access policy.</span></span> 

    <span data-ttu-id="406f3-119">Выполните указанную ниже команду, заменив аргументы **AppId**, **PolicyScopeGroupId** и **Description**.</span><span class="sxs-lookup"><span data-stu-id="406f3-119">Run the following command, replacing the **AppId**, **PolicyScopeGroupId**, and **Description** arguments.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="406f3-120">Протестируйте созданную политику доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="406f3-120">Test the newly created application access policy.</span></span>

    <span data-ttu-id="406f3-121">Выполните указанную ниже команду, заменив аргументы **AppId** и **Identity**.</span><span class="sxs-lookup"><span data-stu-id="406f3-121">Run the following command, replacing the **AppId** and **Identity** arguments.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="406f3-122">В результате выполнения этой команды будет указано, имеет ли приложение доступ к почтовому ящику пользователя User1.</span><span class="sxs-lookup"><span data-stu-id="406f3-122">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

><span data-ttu-id="406f3-123">**Примечание. Чтобы изменения политик доступа приложения вступили в силу в вызовах API Microsoft Graph REST, может потребоваться до 30 минут.**</span><span class="sxs-lookup"><span data-stu-id="406f3-123">**Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.**</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="406f3-124">Поддерживаемые разрешения и дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="406f3-124">Supported permissions and additional resources</span></span>
<span data-ttu-id="406f3-125">Администраторы могут использовать командлеты ApplicationAccessPolicy для управления доступом к почтовым ящикам приложения, которому предоставлены указанные ниже разрешения.</span><span class="sxs-lookup"><span data-stu-id="406f3-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following application permissions:</span></span> 
- <span data-ttu-id="406f3-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="406f3-126">Mail.Read</span></span>
- <span data-ttu-id="406f3-127">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="406f3-127">Mail.ReadBasic</span></span>
- <span data-ttu-id="406f3-128">Mail.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="406f3-128">Mail.ReadBasic.All</span></span>
- <span data-ttu-id="406f3-129">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="406f3-129">Mail.ReadWrite</span></span>
- <span data-ttu-id="406f3-130">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="406f3-130">Mail.Send</span></span>
- <span data-ttu-id="406f3-131">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="406f3-131">MailboxSettings.Read</span></span>  
- <span data-ttu-id="406f3-132">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="406f3-132">MailboxSettings.ReadWrite</span></span>
- <span data-ttu-id="406f3-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="406f3-133">Calendars.Read</span></span>
- <span data-ttu-id="406f3-134">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="406f3-134">Calendars.ReadWrite</span></span>
- <span data-ttu-id="406f3-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="406f3-135">Contacts.Read</span></span>
- <span data-ttu-id="406f3-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="406f3-136">Contacts.ReadWrite</span></span>

<span data-ttu-id="406f3-137">Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="406f3-137">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy).</span></span> 

## <a name="handling-api-errors"></a><span data-ttu-id="406f3-138">Обработка ошибок API</span><span class="sxs-lookup"><span data-stu-id="406f3-138">Handling API errors</span></span>
<span data-ttu-id="406f3-139">Если API-вызову будет отказано в доступе из-за настроек политики доступа приложения, может появиться указанное ниже сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="406f3-139">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
<span data-ttu-id="406f3-140">Если по API-вызовам Microsoft Graph из вашего приложения отображается такое сообщение об ошибке, обратитесь к администратору Exchange Online организации, чтобы убедиться в том, что у вашего приложения есть разрешение на доступ к ресурсу почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="406f3-140">If Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="406f3-141">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="406f3-141">See also</span></span>

- [<span data-ttu-id="406f3-142">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="406f3-142">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="406f3-143">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-143">New-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="406f3-144">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-144">Get-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="406f3-145">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-145">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="406f3-146">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-146">Set-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="406f3-147">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="406f3-147">Test-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/test-applicationaccesspolicy)
