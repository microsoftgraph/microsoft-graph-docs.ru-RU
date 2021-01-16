---
title: Разрешение приложениям доступа к собраниям по сети от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям по сети от имени пользователя.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 856ca755d9eb48aed95139e37a53e2ad420f4250
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882502"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="b1678-103">Разрешение приложениям доступа к собраниям по сети от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="b1678-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="b1678-104">В некоторых случаях, например фоновых службах или приложениях-программах, которые работают на сервере без необходимости вличия пользователя, приложение может вызвать Microsoft Graph, чтобы выполнить действия от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1678-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="b1678-105">Например, приложению может потребоваться вызвать Microsoft Graph для планирования нескольких собраний на основе опубликованных расписаний (например, курсов) или внешних средств планирования.</span><span class="sxs-lookup"><span data-stu-id="b1678-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="b1678-106">В таких случаях пользователь, от имени пользователя, от имени пользователя, будет определен как организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="b1678-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="b1678-107">Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний по сети от имени пользователя, могут использовать для настройки управления доступом **new-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1678-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="b1678-108">В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.</span><span class="sxs-lookup"><span data-stu-id="b1678-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="b1678-109">Эти действия относятся к собраниям по сети и не применимы к другим ресурсам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b1678-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="b1678-110">Настройка политики доступа к приложениям</span><span class="sxs-lookup"><span data-stu-id="b1678-110">Configure application access policy</span></span>

<span data-ttu-id="b1678-111">Чтобы настроить политику доступа к приложениям и разрешить приложениям доступ к собраниям по сети с разрешениями для приложений:</span><span class="sxs-lookup"><span data-stu-id="b1678-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="b1678-112">Определите applcation (client) ID приложения и ИД пользователей, от имени которых приложение будет иметь право на доступ к собраниям по сети.</span><span class="sxs-lookup"><span data-stu-id="b1678-112">Identify the app’s applcation (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="b1678-113">Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="b1678-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="b1678-114">Идентификация пользовательского (объектного) ИД на портале [управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="b1678-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="b1678-115">Подключите к Skype для бизнеса PowerShell с помощью учетной записи администратора.</span><span class="sxs-lookup"><span data-stu-id="b1678-115">Connect to Skype for Business PowerShell with adminitrator account.</span></span> <span data-ttu-id="b1678-116">Подробные сведения см. в под [управлением Skype для бизнеса Online с помощью PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="b1678-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="b1678-117">Создайте политику доступа к приложениям, содержащую список ИД приложения.</span><span class="sxs-lookup"><span data-stu-id="b1678-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="b1678-118">Запустите следующий cmdlet, заменив **аргументы Identity,** **AppIds** и **Description** (необязательно).</span><span class="sxs-lookup"><span data-stu-id="b1678-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="b1678-119">Предоставить пользователю политику, чтобы разрешить содержающимся в ней ИД приложения доступ к собраниям по сети от имени предоставленного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1678-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="b1678-120">Запустите следующий cmdlet, заменив **аргументы PolicyName** и **Identity.**</span><span class="sxs-lookup"><span data-stu-id="b1678-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> <span data-ttu-id="b1678-121">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="b1678-121">**Note**</span></span> 
> 
> - <span data-ttu-id="b1678-122">_Идентификатор_ ссылается на имя политики при создании политики, но идентификатор пользователя при ее предоставлении.</span><span class="sxs-lookup"><span data-stu-id="b1678-122">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="b1678-123">Изменение политик доступа к приложениям может занять до 30 минут, чтобы внести изменения в вызовы REST API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b1678-123">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="b1678-124">Поддерживаемые разрешения и дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="b1678-124">Supported permissions and additional resources</span></span>

<span data-ttu-id="b1678-125">Администраторы могут использовать cmdlets ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которое имеет любое из следующих разрешений приложения:</span><span class="sxs-lookup"><span data-stu-id="b1678-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="b1678-126">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1678-126">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="b1678-127">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1678-127">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="b1678-128">Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="b1678-128">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="b1678-129">Ошибки</span><span class="sxs-lookup"><span data-stu-id="b1678-129">Errors</span></span>

<span data-ttu-id="b1678-130">Если вызову API отказано в доступе из-за того, что приложение пытается получить доступ к собранию по сети, если политика доступа к приложению не настроена, может возникнуть следующая ошибка.</span><span class="sxs-lookup"><span data-stu-id="b1678-130">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="b1678-131">Следуйте шагам в этой статье, чтобы создать и/или предоставить политику доступа к приложениям, которая содержит ИД приложения для ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1678-131">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="b1678-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b1678-132">See also</span></span>

- [<span data-ttu-id="b1678-133">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="b1678-133">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="b1678-134">New-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1678-134">New-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="b1678-135">Grant-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1678-135">Grant-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="b1678-136">Get-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1678-136">Get-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="b1678-137">Set-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1678-137">Set-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="b1678-138">Remove-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1678-138">Remove-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
