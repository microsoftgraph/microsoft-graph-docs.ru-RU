---
title: Управление номерами телефонов для ботов
description: В этой статье описывается создание бота, который можно достичь с помощью номера телефона.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: d6b71d2db1be951137ca33026f243dae6055c93f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573574"
---
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="722d2-103">Управление номерами телефонов для ботов</span><span class="sxs-lookup"><span data-stu-id="722d2-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="722d2-104">В этой статье описывается создание бота, который можно достичь с помощью номера телефона.</span><span class="sxs-lookup"><span data-stu-id="722d2-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="722d2-105">При создании бота будет полезно ознакомиться со следующими терминами:</span><span class="sxs-lookup"><span data-stu-id="722d2-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="722d2-106">**Application** — приложение, которое находится в Azure, также именуемом **ботом.**</span><span class="sxs-lookup"><span data-stu-id="722d2-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="722d2-107">**Пример приложения** — объект с отключенным пользователем, который может быть назначен номеру телефона, который может использоваться ботом.</span><span class="sxs-lookup"><span data-stu-id="722d2-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="722d2-108">Это также называется учетной [записью ресурса.](/microsoftteams/manage-resource-accounts)</span><span class="sxs-lookup"><span data-stu-id="722d2-108">This is also known as a [resource account](/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="722d2-109">Это единственный способ присвоения номера телефона боту.</span><span class="sxs-lookup"><span data-stu-id="722d2-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="722d2-110">Одно приложение может иметь несколько экземпляров приложений, а каждый клиент может иметь несколько экземпляров приложений, как показано на следующем изображении.</span><span class="sxs-lookup"><span data-stu-id="722d2-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![Изображение, на котором показан номер телефона с клиентом с одним или более экземплярами приложений](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="722d2-112">Обязательное условие — регистрация бота</span><span class="sxs-lookup"><span data-stu-id="722d2-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="722d2-113">Чтобы начать работу, следуйте инструкциям по регистрации [вызываемого бота.](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)</span><span class="sxs-lookup"><span data-stu-id="722d2-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="722d2-114">Для использования в коде вам потребуется использовать конфигуративные значения, такие как код бота, код приложения Майкрософт и пароль приложения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="722d2-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="722d2-115">Добавьте следующие разрешения в бот.</span><span class="sxs-lookup"><span data-stu-id="722d2-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="722d2-116">Администратору клиента также необходимо дать согласие на эти разрешения:</span><span class="sxs-lookup"><span data-stu-id="722d2-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="722d2-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="722d2-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="722d2-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="722d2-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="722d2-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="722d2-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="722d2-120">Calls.JoinGroupCallAsGuest.All</span><span class="sxs-lookup"><span data-stu-id="722d2-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="722d2-121">Дополнительные сведения о разрешениях, связанных с вызовами, см. в справке [Permissions.](permissions-reference.md#calls-permissions)</span><span class="sxs-lookup"><span data-stu-id="722d2-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="722d2-122">Назначение номера телефона боту</span><span class="sxs-lookup"><span data-stu-id="722d2-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="722d2-123">Назначение номера телефона боту включает в себя три действия:</span><span class="sxs-lookup"><span data-stu-id="722d2-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="722d2-124">Создание экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="722d2-124">Create an application instance.</span></span>
2.  <span data-ttu-id="722d2-125">Назначение лицензий Microsoft 365 экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="722d2-125">Assign Microsoft 365 licenses to your application instance.</span></span>
3.  <span data-ttu-id="722d2-126">Назначьте номер телефона экземпляру приложения (только администратору клиента).</span><span class="sxs-lookup"><span data-stu-id="722d2-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="722d2-127">Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="722d2-127">Create an application instance</span></span>

<span data-ttu-id="722d2-128">Если он еще не установлен, администратору клиента необходимо установить [модуль Skype для бизнеса Online для](https://www.microsoft.com/download/details.aspx?id=39366) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="722d2-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="722d2-129">Администратор клиента должен войти с помощью учетных данных перед запуском cmdlet.</span><span class="sxs-lookup"><span data-stu-id="722d2-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="722d2-130">Чтобы создать новый экземпляр приложения, администратор клиента запускает следующий кодлет.</span><span class="sxs-lookup"><span data-stu-id="722d2-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

<span data-ttu-id="722d2-131">При создания экземпляра приложения используйте комлет синхронизации.</span><span class="sxs-lookup"><span data-stu-id="722d2-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="722d2-132">Дополнительные сведения см. [в new-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="722d2-132">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a><span data-ttu-id="722d2-133">Назначение лицензий Microsoft 365 экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="722d2-133">Assign Microsoft 365 licenses to your application instance</span></span>

<span data-ttu-id="722d2-134">Назначение виртуальной пользовательской лицензии экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="722d2-134">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="722d2-135">Подробные сведения см. в [материале Phone system virtual user license.](/microsoftteams/teams-add-on-licensing/virtual-user)</span><span class="sxs-lookup"><span data-stu-id="722d2-135">For details, see [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

<span data-ttu-id="722d2-136">Назначение плана вызова экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="722d2-136">Assign a calling plan to your application instance.</span></span> <span data-ttu-id="722d2-137">Подробные сведения [см. в материале Calling plans for Microsoft 365.](/microsoftteams/calling-plans-for-office-365)</span><span class="sxs-lookup"><span data-stu-id="722d2-137">For details, see [Calling plans for Microsoft 365](/microsoftteams/calling-plans-for-office-365).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="722d2-138">Назначение номера телефона экземпляру приложения (только администратору клиента)</span><span class="sxs-lookup"><span data-stu-id="722d2-138">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="722d2-139">Прежде чем выполнить настройку пользователей в пределах своей организации на осуществление и прием звонков, необходимо получить телефонные номера для них.</span><span class="sxs-lookup"><span data-stu-id="722d2-139">Before you can set up users in your organization to make and receive phone calls, you must get phone numbers for them.</span></span> <span data-ttu-id="722d2-140">Подробные сведения см. [в материале Получение номеров телефонов для пользователей.](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users)</span><span class="sxs-lookup"><span data-stu-id="722d2-140">For details, see [Getting phone numbers for your users](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).</span></span>

<span data-ttu-id="722d2-141">Чтобы назначить номер телефона экземпляру приложения, администратор клиента:</span><span class="sxs-lookup"><span data-stu-id="722d2-141">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="722d2-142">Войт в центр администрирования Teams в качестве администратора клиента.</span><span class="sxs-lookup"><span data-stu-id="722d2-142">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="722d2-143">Переходит на **номера голосовых телефонов Центра**  >    >  **администрирования** Teams.</span><span class="sxs-lookup"><span data-stu-id="722d2-143">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="722d2-144">Назначает номер телефона службы (+11D-формат) с помощью следующего cmdlet.</span><span class="sxs-lookup"><span data-stu-id="722d2-144">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
<span data-ttu-id="722d2-145">При присвоении номера телефона службы используйте комлет синхронизации.</span><span class="sxs-lookup"><span data-stu-id="722d2-145">When the service phone number is assigned, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="722d2-146">Дополнительные сведения см. [в рублях Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="722d2-146">For more information, see [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="722d2-147">Отозвание номера телефона бота</span><span class="sxs-lookup"><span data-stu-id="722d2-147">Unassign a bot phone number</span></span>

<span data-ttu-id="722d2-148">Чтобы отогнать номер телефона, используйте следующий комдлет.</span><span class="sxs-lookup"><span data-stu-id="722d2-148">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="722d2-149">**Примечание:** В настоящее время это работает только с онлайн-номерами, а не с номерами прямой маршрутики (DR).</span><span class="sxs-lookup"><span data-stu-id="722d2-149">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="722d2-150">Это известная проблема.</span><span class="sxs-lookup"><span data-stu-id="722d2-150">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="722d2-151">Обновление номера телефона бота</span><span class="sxs-lookup"><span data-stu-id="722d2-151">Update a bot phone number</span></span>

<span data-ttu-id="722d2-152">После отвода номера можно назначить боту другой номер с помощью следующего cmdlet.</span><span class="sxs-lookup"><span data-stu-id="722d2-152">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="722d2-153">См. также</span><span class="sxs-lookup"><span data-stu-id="722d2-153">See also</span></span>

- <span data-ttu-id="722d2-154">[Пример бота инцидента](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span><span class="sxs-lookup"><span data-stu-id="722d2-154">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="722d2-155">Дополнительные сведения о развертывании см. в [примере Deploying the sample.](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)</span><span class="sxs-lookup"><span data-stu-id="722d2-155">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>
