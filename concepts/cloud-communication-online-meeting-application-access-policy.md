---
title: Разрешение приложениям получать доступ к собраниям по сети от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям по сети от имени пользователя.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a0a0d264e8898d8524f104d3fe5dafeb1b151f5f
ms.sourcegitcommit: 6eadb95e21b2e7eb5d6b081b91999cb91070f397
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2020
ms.locfileid: "48299272"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="3c18d-103">Разрешение приложениям получать доступ к собраниям по сети от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="3c18d-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="3c18d-104">В некоторых случаях, например, для фоновых служб или приложений-демонов, выполняемых на сервере без присутствия вошедшего пользователя, приложение может вызвать Microsoft Graph для выполнения действий от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c18d-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="3c18d-105">Например, приложению может потребоваться вызвать Microsoft Graph, чтобы спланировать несколько собраний на основе опубликованных расписаний (таких как курсы) или внешних средств планирования.</span><span class="sxs-lookup"><span data-stu-id="3c18d-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="3c18d-106">В таких случаях пользователь, работающий с приложением от имени, идентифицируется в качестве организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="3c18d-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="3c18d-107">Администраторы, которые хотят разрешить приложению получать доступ к ресурсам собраний по сети от имени пользователя, могут использовать командлеты PowerShell **New-ксаппликатионакцессполици** и **Grant-ксаппликатионакцессполици** для настройки управления доступом.</span><span class="sxs-lookup"><span data-stu-id="3c18d-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="3c18d-108">В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="3c18d-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="3c18d-109">Эти действия относятся только к собраниям по сети и не распространяются на другие ресурсы Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3c18d-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="3c18d-110">Настройка политики доступа к приложениям</span><span class="sxs-lookup"><span data-stu-id="3c18d-110">Configure application access policy</span></span>

<span data-ttu-id="3c18d-111">Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям по сети с разрешениями для приложений:</span><span class="sxs-lookup"><span data-stu-id="3c18d-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="3c18d-112">Определите апплкатион (Client) ID приложения и идентификаторы пользователей, от имени которых приложение будет авторизовано для доступа к собраниям по сети.</span><span class="sxs-lookup"><span data-stu-id="3c18d-112">Identify the app’s applcation (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="3c18d-113">Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="3c18d-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="3c18d-114">Определение идентификатора пользователя (объекта) пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="3c18d-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="3c18d-115">Подключитесь к Skype для бизнеса PowerShell с помощью учетной записи админитратор.</span><span class="sxs-lookup"><span data-stu-id="3c18d-115">Connect to Skype for Business PowerShell with adminitrator account.</span></span> <span data-ttu-id="3c18d-116">Дополнительные сведения: [Управление Skype для бизнеса Online с помощью PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="3c18d-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="3c18d-117">Создайте политику доступа к приложениям, содержащую список идентификаторов приложений.</span><span class="sxs-lookup"><span data-stu-id="3c18d-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="3c18d-118">Выполните следующий командлет, заменив аргументы **Identity**, **AppID**и **Description** (необязательный параметр).</span><span class="sxs-lookup"><span data-stu-id="3c18d-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="3c18d-119">Предоставьте политике пользователю разрешение на доступ к собраниям по сети от имени предоставленного пользователя с помощью идентификаторов приложений, включенных в политику.</span><span class="sxs-lookup"><span data-stu-id="3c18d-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="3c18d-120">Выполните следующий командлет, заменив аргументы **PolicyName** и **Identity** .</span><span class="sxs-lookup"><span data-stu-id="3c18d-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> <span data-ttu-id="3c18d-121">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="3c18d-121">**Note**</span></span> 
> 
> - <span data-ttu-id="3c18d-122">_Identity_ — это имя политики при создании политики, но идентификатор пользователя при предоставлении политики.</span><span class="sxs-lookup"><span data-stu-id="3c18d-122">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="3c18d-123">Для вступления в силу изменений в политиках доступа к приложениям в вызовах REST API Microsoft Graph может потребоваться до 30 минут.</span><span class="sxs-lookup"><span data-stu-id="3c18d-123">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="3c18d-124">Поддерживаемые разрешения и дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="3c18d-124">Supported permissions and additional resources</span></span>

<span data-ttu-id="3c18d-125">Администраторы могут использовать командлеты Аппликатионакцессполици для управления доступом к почтовым ящикам для приложения, которому предоставлено одно из следующих разрешений приложения:</span><span class="sxs-lookup"><span data-stu-id="3c18d-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="3c18d-126">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c18d-126">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="3c18d-127">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c18d-127">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="3c18d-128">Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="3c18d-128">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="3c18d-129">Ошибки</span><span class="sxs-lookup"><span data-stu-id="3c18d-129">Errors</span></span>

<span data-ttu-id="3c18d-130">Если в вызове API отказано в доступе из-за того, что приложение пытается получить доступ к собранию по сети, когда политика доступа к приложениям не настроена, может возникнуть следующая ошибка.</span><span class="sxs-lookup"><span data-stu-id="3c18d-130">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

```json
{
    "error": {
        "code": "Unauthorized",
        "message": "App <app_ID_redacted> is not authorized to Create meeting on behalf of user <user_ID_redacted>",
        "innerError": {
            "date": "<date_redacted>",
            "request-id": "599d9cb0-56ac-4dc5-b6f8-1456a1414609"
        }
    }
}
```

<span data-ttu-id="3c18d-131">Выполните действия, описанные в этой статье, чтобы создать и/или предоставить политику доступа к приложению, содержащую идентификатор приложения, в идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c18d-131">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="3c18d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="3c18d-132">See also</span></span>

- [<span data-ttu-id="3c18d-133">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="3c18d-133">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="3c18d-134">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3c18d-134">New-ApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="3c18d-135">Granting — Аппликатионакцессполици</span><span class="sxs-lookup"><span data-stu-id="3c18d-135">Grant-ApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="3c18d-136">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3c18d-136">Get-ApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="3c18d-137">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3c18d-137">Set-ApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="3c18d-138">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3c18d-138">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
