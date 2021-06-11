---
title: Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям в Интернете от имени пользователя.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: fa3771c1325f0c2a5f10b425e2eca51e9d1534ac
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896706"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="a34b7-103">Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="a34b7-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="a34b7-104">В некоторых случаях, например в фоновых службах или приложениях daemon, которые работают на сервере без присутствия подписанного пользователя, приложение может вызвать microsoft Graph, чтобы принять меры от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="a34b7-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="a34b7-105">Например, приложению может потребоваться вызвать microsoft Graph, чтобы запланировать несколько собраний, основанных на опубликованных расписаниях (например, курсах) или внешних средствах планирования.</span><span class="sxs-lookup"><span data-stu-id="a34b7-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="a34b7-106">В этих случаях пользователь, который действует от имени приложения, определен как организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="a34b7-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="a34b7-107">Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний в Интернете от имени пользователя, могут использовать команды **New-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell для настройки управления доступом.</span><span class="sxs-lookup"><span data-stu-id="a34b7-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="a34b7-108">В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="a34b7-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="a34b7-109">Эти действия относятся к собраниям в Интернете и не применяются к другим Graph Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a34b7-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="a34b7-110">Настройка политики доступа к приложениям</span><span class="sxs-lookup"><span data-stu-id="a34b7-110">Configure application access policy</span></span>

<span data-ttu-id="a34b7-111">Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям в Интернете с разрешениями приложений:</span><span class="sxs-lookup"><span data-stu-id="a34b7-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="a34b7-112">Определите ID приложения (клиента) и пользовательские ИД пользователей, от имени которых приложение будет уполномочено получать доступ к собраниям в Интернете.</span><span class="sxs-lookup"><span data-stu-id="a34b7-112">Identify the app’s application (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="a34b7-113">Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="a34b7-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="a34b7-114">Идентификация пользователя (объекта) на портале управления пользователями [Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="a34b7-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="a34b7-115">Подключение Skype для бизнеса PowerShell с учетной записью администратора.</span><span class="sxs-lookup"><span data-stu-id="a34b7-115">Connect to Skype for Business PowerShell with an administrator account.</span></span> <span data-ttu-id="a34b7-116">Подробные сведения см. в [Skype для бизнеса Управление Skype для бизнеса с PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="a34b7-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="a34b7-117">Создайте политику доступа к приложениям, содержащую список ID приложений.</span><span class="sxs-lookup"><span data-stu-id="a34b7-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="a34b7-118">Запустите следующий cmdlet, заменив **аргументы Identity,** **AppIds** и **Description** (необязательный).</span><span class="sxs-lookup"><span data-stu-id="a34b7-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="a34b7-119">Предоставление политики пользователю, чтобы позволить ID-данным приложения, содержающимся в политике, получать доступ к собраниям в Интернете от имени предоставленного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a34b7-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="a34b7-120">Запустите следующий комдлет, заменив **аргументы PolicyName** и **Identity.**</span><span class="sxs-lookup"><span data-stu-id="a34b7-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> [!NOTE]
> - <span data-ttu-id="a34b7-121">_Identity_ ссылается на имя политики при создании политики, но идентификатор пользователя при предоставлении политики.</span><span class="sxs-lookup"><span data-stu-id="a34b7-121">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="a34b7-122">Изменение политик доступа к приложениям может занять до 30 минут для звонков microsoft Graph API REST.</span><span class="sxs-lookup"><span data-stu-id="a34b7-122">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="a34b7-123">Поддерживаемые разрешения и дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="a34b7-123">Supported permissions and additional resources</span></span>

<span data-ttu-id="a34b7-124">Администраторы могут использовать cmdlets ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которое было предоставлено любое из следующих разрешений приложения:</span><span class="sxs-lookup"><span data-stu-id="a34b7-124">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="a34b7-125">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a34b7-125">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="a34b7-126">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a34b7-126">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="a34b7-127">Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="a34b7-127">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="a34b7-128">Ошибки</span><span class="sxs-lookup"><span data-stu-id="a34b7-128">Errors</span></span>

<span data-ttu-id="a34b7-129">Вы можете столкнуться со следующей ошибкой, когда вызову API отказано в доступе из-за того, что приложение пытается получить доступ к собранию в Интернете, если политика доступа к приложениям не настроена.</span><span class="sxs-lookup"><span data-stu-id="a34b7-129">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="a34b7-130">Следуйте шагам в этой статье, чтобы создать и/или предоставить политику доступа к приложениям, которая содержит ID приложения для пользовательского ИД.</span><span class="sxs-lookup"><span data-stu-id="a34b7-130">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="a34b7-131">См. также</span><span class="sxs-lookup"><span data-stu-id="a34b7-131">See also</span></span>

- [<span data-ttu-id="a34b7-132">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="a34b7-132">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="a34b7-133">New-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a34b7-133">New-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="a34b7-134">Grant-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a34b7-134">Grant-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="a34b7-135">Get-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a34b7-135">Get-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="a34b7-136">Set-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a34b7-136">Set-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="a34b7-137">Remove-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a34b7-137">Remove-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
