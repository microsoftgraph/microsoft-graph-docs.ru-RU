---
title: Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям в Интернете от имени пользователя.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ff14ae4506cc19adf58ab61cde436a0252bd6f5c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920399"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="a52fd-103">Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="a52fd-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="a52fd-104">В некоторых случаях, например в фоновых службах или приложениях daemon, которые работают на сервере без присутствия подписанного пользователя, приложение может вызвать Microsoft Graph для действий от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="a52fd-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="a52fd-105">Например, приложению может потребоваться вызвать Microsoft Graph, чтобы запланировать несколько собраний на основе опубликованных расписания (например, курсов) или внешних средств планирования.</span><span class="sxs-lookup"><span data-stu-id="a52fd-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="a52fd-106">В этих случаях пользователь, который действует от имени приложения, определен как организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="a52fd-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="a52fd-107">Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний в Интернете от имени пользователя, могут использовать команды **New-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell для настройки управления доступом.</span><span class="sxs-lookup"><span data-stu-id="a52fd-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="a52fd-108">В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="a52fd-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="a52fd-109">Эти действия относятся к собраниям в Интернете и не применяются к другим ресурсам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a52fd-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="a52fd-110">Настройка политики доступа к приложениям</span><span class="sxs-lookup"><span data-stu-id="a52fd-110">Configure application access policy</span></span>

<span data-ttu-id="a52fd-111">Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям в Интернете с разрешениями приложений:</span><span class="sxs-lookup"><span data-stu-id="a52fd-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="a52fd-112">Определите ID приложения (клиента) и пользовательские ИД пользователей, от имени которых приложение будет уполномочено получать доступ к собраниям в Интернете.</span><span class="sxs-lookup"><span data-stu-id="a52fd-112">Identify the app’s application (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="a52fd-113">Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="a52fd-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="a52fd-114">Идентификация пользователя (объекта) на портале управления пользователями [Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="a52fd-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="a52fd-115">Подключение к Skype для бизнеса PowerShell с учетной записью администратора.</span><span class="sxs-lookup"><span data-stu-id="a52fd-115">Connect to Skype for Business PowerShell with an administrator account.</span></span> <span data-ttu-id="a52fd-116">Подробные сведения см. [в материале Управление Skype для бизнеса Online с помощью PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="a52fd-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="a52fd-117">Создайте политику доступа к приложениям, содержащую список ID приложений.</span><span class="sxs-lookup"><span data-stu-id="a52fd-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="a52fd-118">Запустите следующий cmdlet, заменив **аргументы Identity,** **AppIds** и **Description** (необязательный).</span><span class="sxs-lookup"><span data-stu-id="a52fd-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="a52fd-119">Предоставление политики пользователю, чтобы позволить ID-данным приложения, содержающимся в политике, получать доступ к собраниям в Интернете от имени предоставленного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a52fd-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="a52fd-120">Запустите следующий комдлет, заменив **аргументы PolicyName** и **Identity.**</span><span class="sxs-lookup"><span data-stu-id="a52fd-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> [!NOTE]
> - <span data-ttu-id="a52fd-121">_Identity_ ссылается на имя политики при создании политики, но идентификатор пользователя при предоставлении политики.</span><span class="sxs-lookup"><span data-stu-id="a52fd-121">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="a52fd-122">Изменение политик доступа к приложениям может занять до 30 минут, чтобы внести изменения в API API MICROSOFT Graph REST.</span><span class="sxs-lookup"><span data-stu-id="a52fd-122">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="a52fd-123">Поддерживаемые разрешения и дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="a52fd-123">Supported permissions and additional resources</span></span>

<span data-ttu-id="a52fd-124">Администраторы могут использовать cmdlets ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которое было предоставлено любое из следующих разрешений приложения:</span><span class="sxs-lookup"><span data-stu-id="a52fd-124">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="a52fd-125">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a52fd-125">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="a52fd-126">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52fd-126">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="a52fd-127">Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="a52fd-127">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="a52fd-128">Ошибки</span><span class="sxs-lookup"><span data-stu-id="a52fd-128">Errors</span></span>

<span data-ttu-id="a52fd-129">Вы можете столкнуться со следующей ошибкой, когда вызову API отказано в доступе из-за того, что приложение пытается получить доступ к собранию в Интернете, если политика доступа к приложениям не настроена.</span><span class="sxs-lookup"><span data-stu-id="a52fd-129">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="a52fd-130">Следуйте шагам в этой статье, чтобы создать и/или предоставить политику доступа к приложениям, которая содержит ID приложения для пользовательского ИД.</span><span class="sxs-lookup"><span data-stu-id="a52fd-130">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="a52fd-131">См. также</span><span class="sxs-lookup"><span data-stu-id="a52fd-131">See also</span></span>

- [<span data-ttu-id="a52fd-132">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="a52fd-132">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="a52fd-133">New-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a52fd-133">New-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="a52fd-134">Grant-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a52fd-134">Grant-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="a52fd-135">Get-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a52fd-135">Get-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="a52fd-136">Set-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a52fd-136">Set-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="a52fd-137">Remove-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a52fd-137">Remove-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
