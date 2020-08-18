---
title: Управление номерами телефонов для ботов
description: В этой статье описывается, как создать робот, достижимый через телефонный номер.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 2dc201ff9423b0190daa5adf86871972cc577304
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792872"
---
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="a1ade-103">Управление номерами телефонов для ботов</span><span class="sxs-lookup"><span data-stu-id="a1ade-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="a1ade-104">В этой статье описывается, как создать робот, достижимый через телефонный номер.</span><span class="sxs-lookup"><span data-stu-id="a1ade-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="a1ade-105">По мере создания ленты вам будет полезно ознакомиться со следующими терминами:</span><span class="sxs-lookup"><span data-stu-id="a1ade-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="a1ade-106">**Приложение** — приложение, размещенное в Azure, которое также называется " **Bot**".</span><span class="sxs-lookup"><span data-stu-id="a1ade-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="a1ade-107">**Экземпляр приложения** — объект отключенного пользователя, который может быть назначен телефонному номеру, который может использоваться с помощью Bot.</span><span class="sxs-lookup"><span data-stu-id="a1ade-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="a1ade-108">Это также называется [учетной записью ресурса](https://docs.microsoft.com/microsoftteams/manage-resource-accounts).</span><span class="sxs-lookup"><span data-stu-id="a1ade-108">This is also known as a [resource account](https://docs.microsoft.com/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="a1ade-109">Это единственный способ, которым можно назначить номер телефона для ленты.</span><span class="sxs-lookup"><span data-stu-id="a1ade-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="a1ade-110">Одно приложение может иметь несколько экземпляров приложений, и каждый клиент может иметь несколько экземпляров приложения, как показано на следующем рисунке.</span><span class="sxs-lookup"><span data-stu-id="a1ade-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![Изображение номера телефона с клиентами с одним или несколькими экземплярами приложений](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="a1ade-112">Обязательное требование: регистрация Bot</span><span class="sxs-lookup"><span data-stu-id="a1ade-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="a1ade-113">Чтобы приступить к работе, выполните инструкции по [регистрации абонентского робота](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span><span class="sxs-lookup"><span data-stu-id="a1ade-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="a1ade-114">Вам понадобятся значения конфигурации, такие как ИДЕНТИФИКАТОРы Bot, идентификатор приложения и пароль Microsoft App, чтобы использовать их в вашем коде.</span><span class="sxs-lookup"><span data-stu-id="a1ade-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="a1ade-115">Добавьте указанные ниже разрешения для ленты.</span><span class="sxs-lookup"><span data-stu-id="a1ade-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="a1ade-116">Администратору клиента необходимо также предоставить разрешения для этих разрешений:</span><span class="sxs-lookup"><span data-stu-id="a1ade-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="a1ade-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a1ade-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="a1ade-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="a1ade-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="a1ade-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="a1ade-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="a1ade-120">Calls. Жоинграупкалласгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="a1ade-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="a1ade-121">Дополнительные сведения о разрешениях, связанных с вызовами, приведены в статье [References](permissions-reference.md#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="a1ade-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="a1ade-122">Назначение номера телефона для ленты</span><span class="sxs-lookup"><span data-stu-id="a1ade-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="a1ade-123">Назначение номера телефона для ленты состоит из трех этапов:</span><span class="sxs-lookup"><span data-stu-id="a1ade-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="a1ade-124">Создайте экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="a1ade-124">Create an application instance.</span></span>
2.  <span data-ttu-id="a1ade-125">Назначьте для экземпляра приложения лицензию виртуального пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1ade-125">Assign a virtual user license to your application instance.</span></span>
3.  <span data-ttu-id="a1ade-126">Назначить номер телефона экземпляру приложения (только администратор клиента).</span><span class="sxs-lookup"><span data-stu-id="a1ade-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="a1ade-127">Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="a1ade-127">Create an application instance</span></span>

<span data-ttu-id="a1ade-128">Если он еще не установлен, администратору клиента необходимо установить [модуль Skype для бизнеса Online](https://www.microsoft.com/download/details.aspx?id=39366) для PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a1ade-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="a1ade-129">Перед выполнением командлета администратор клиента должен войти в систему, используя свои учетные данные.</span><span class="sxs-lookup"><span data-stu-id="a1ade-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="a1ade-130">Для создания нового экземпляра приложения администратор клиента выполняет следующий командлет.</span><span class="sxs-lookup"><span data-stu-id="a1ade-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId “<app_id>” -DisplayName "<bot_display_name>"`

<span data-ttu-id="a1ade-131">При создании экземпляра приложения используйте командлет Sync.</span><span class="sxs-lookup"><span data-stu-id="a1ade-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

### <a name="assign-a-virtual-user-license-to-your-application-instance"></a><span data-ttu-id="a1ade-132">Назначение лицензии виртуального пользователя экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="a1ade-132">Assign a virtual user license to your application instance</span></span>

<span data-ttu-id="a1ade-133">Назначьте для экземпляра приложения лицензию виртуального пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1ade-133">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="a1ade-134">Дополнительную информацию можно узнать в статье [Лицензия виртуального пользователя телефонной системы](https://docs.microsoft.com/microsoftteams/teams-add-on-licensing/virtual-user).</span><span class="sxs-lookup"><span data-stu-id="a1ade-134">For details, see [Phone system virtual user license](https://docs.microsoft.com/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="a1ade-135">Назначение номера телефона экземпляру приложения (только администратор клиента)</span><span class="sxs-lookup"><span data-stu-id="a1ade-135">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="a1ade-136">Чтобы назначить номер телефона экземпляру приложения, администратор клиента:</span><span class="sxs-lookup"><span data-stu-id="a1ade-136">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="a1ade-137">Вход в центр администрирования Teams в качестве администратора клиента.</span><span class="sxs-lookup"><span data-stu-id="a1ade-137">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="a1ade-138">Передается на голосовые телефоны **центра администрирования Teams**  >  **Voice**  >  **Phone Numbers**.</span><span class="sxs-lookup"><span data-stu-id="a1ade-138">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="a1ade-139">Назначает номер телефона службы (формат 11D) с помощью следующего командлета.</span><span class="sxs-lookup"><span data-stu-id="a1ade-139">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="a1ade-140">Отмена назначения номера телефона для ленты</span><span class="sxs-lookup"><span data-stu-id="a1ade-140">Unassign a bot phone number</span></span>

<span data-ttu-id="a1ade-141">Используйте следующий командлет, чтобы отменить назначение номера телефона.</span><span class="sxs-lookup"><span data-stu-id="a1ade-141">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="a1ade-142">**Примечание:** В настоящее время это работает только с номерами в сети, а не с номерами аварийной маршрутизации (DR).</span><span class="sxs-lookup"><span data-stu-id="a1ade-142">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="a1ade-143">Это известная проблема.</span><span class="sxs-lookup"><span data-stu-id="a1ade-143">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="a1ade-144">Обновление номера телефона для ленты</span><span class="sxs-lookup"><span data-stu-id="a1ade-144">Update a bot phone number</span></span>

<span data-ttu-id="a1ade-145">После этого вы можете назначить себе другой номер с помощью следующего командлета.</span><span class="sxs-lookup"><span data-stu-id="a1ade-145">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="a1ade-146">См. также</span><span class="sxs-lookup"><span data-stu-id="a1ade-146">See also</span></span>

- <span data-ttu-id="a1ade-147">[Пример ленты для инцидента](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span><span class="sxs-lookup"><span data-stu-id="a1ade-147">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="a1ade-148">Сведения о развертывании можно найти в статье [развертывание примера](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span><span class="sxs-lookup"><span data-stu-id="a1ade-148">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>

