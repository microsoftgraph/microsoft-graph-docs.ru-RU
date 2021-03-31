---
title: Получение уведомлений об изменениях разными способами
description: Уведомления об изменениях можно получать с помощью разных технологий, включая веб-перехватчики и концентраторы событий Azure.
author: Jumaodhiss
localization_priority: Priority
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 2cb6000b309b9bcaf5af840cc26976c7254d2d96
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469103"
---
# <a name="get-change-notifications-delivered-in-different-ways-preview"></a><span data-ttu-id="6b3f0-103">Получение уведомлений об изменениях разными способами (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6b3f0-103">Get change notifications delivered in different ways (preview)</span></span>

<span data-ttu-id="6b3f0-104">Уведомления об изменениях можно отправлять подписчикам разными способами.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-104">Change notifications can be delivered in different ways to subscribers.</span></span> <span data-ttu-id="6b3f0-105">Если основной способ доставки уведомлений об изменениях — веб-перехватчики, может оказаться непросто использовать их преимущества в условиях высокой пропускной способности или когда получатель не может предоставить общедоступный URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-105">If the main delivery mode for change notifications is through webhooks, it can be challenging to take advantage of webhooks for high throughput scenarios or when the receiver cannot expose a publicly available notification URL.</span></span>  

<span data-ttu-id="6b3f0-106">Этот способ доставки уведомлений об изменениях доступен для всех ресурсов, поддерживающих уведомления об изменениях Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-106">This change notifications delivery mode is available for all resources that support Microsoft Graph change notifications.</span></span>

<span data-ttu-id="6b3f0-107">Ниже приведены примеры сценариев с высокой пропускной способностью, в том числе приложения, которые подписаны на многие ресурсы, приложения, которые подписаны на часто изменяющиеся ресурсы, и многоуровневые приложения, которые подписаны на ресурсы в рамках большого набора организаций.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-107">Good examples of high throughput scenarios include applications subscribing to a large set of resources, applications subscribing to resources that change with a high frequency, and multi-tenant applications that subscribe to resources accross a large set of organizations.</span></span>

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a><span data-ttu-id="6b3f0-108">Получение уведомлений об изменениях с помощью концентраторов событий Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f0-108">Using Azure Event Hubs to receive change notifications</span></span>

<span data-ttu-id="6b3f0-109">[Концентраторы событий Azure](https://azure.microsoft.com/services/event-hubs) — это сервис приема и распространения популярных событий в режиме реального времени, созданный для масштабирования.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-109">[Azure Event Hubs](https://azure.microsoft.com/services/event-hubs) is a popular real-time events ingestion and distribution service built for scale.</span></span> <span data-ttu-id="6b3f0-110">Для получения уведомлений об изменениях вместо традиционных веб-перехватчиков можно использовать концентраторы событий Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-110">You can use Azure Events Hubs instead of traditional webhooks to receive change notifications.</span></span> <span data-ttu-id="6b3f0-111">В настоящее время эта функция находится на стадии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-111">This feature is currently in preview.</span></span>  
<span data-ttu-id="6b3f0-112">Использование концентраторов событий Azure для получения уведомлений о изменениях отличается от веб-перехватчиков несколькими моментами, в том числе:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-112">Using Azure Event Hubs to receive change notifications differs from webhooks in a few ways, including:</span></span>

- <span data-ttu-id="6b3f0-113">Не приходится полагаться на общедоступные URL-адреса уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-113">You don't rely on publicly exposed notification URLs.</span></span> <span data-ttu-id="6b3f0-114">Пакет SDK концентраторов событий ретранслирует уведомления в ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-114">The Event Hubs SDK will relay the notifications to your application.</span></span>
- <span data-ttu-id="6b3f0-115">Нет необходимости отвечать на [проверку URL-адреса уведомлений](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="6b3f0-115">You don't need to reply to the [notification URL validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="6b3f0-116">Можно пропустить полученное сообщение о проверке.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-116">You can ignore the validation message that you receive.</span></span>
- <span data-ttu-id="6b3f0-117">Необходимо подготовить концентратор событий Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-117">You'll need to provision an Azure Event Hub.</span></span>
- <span data-ttu-id="6b3f0-118">Необходимо подготовить хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-118">You'll need to provision an Azure Key Vault.</span></span>

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a><span data-ttu-id="6b3f0-119">Настройка хранилища Azure Key Vault и концентраторов событий Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f0-119">Set up the Azure KeyVault and Azure Event Hubs</span></span>

<span data-ttu-id="6b3f0-120">В этом разделе вы узнаете, как выполнить настройку обязательных служб Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-120">This section will walk you through the setup of required Azure services.</span></span>

#### <a name="option-1-using-the-azure-cli"></a><span data-ttu-id="6b3f0-121">Вариант 1: использование CLI</span><span class="sxs-lookup"><span data-stu-id="6b3f0-121">Option 1: Using the Azure CLI</span></span>

<span data-ttu-id="6b3f0-122">Средство [Azure CLI](/cli/azure/what-is-azure-cli) позволяет создавать сценарии и автоматизировать админстративные задачи в Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-122">The [Azure CLI](/cli/azure/what-is-azure-cli) allows you to script and automate adminstrative tasks in Azure.</span></span> <span data-ttu-id="6b3f0-123">Средство CLI можно [установить на локальный компьютер](/cli/azure/install-azure-cli) или запустить напрямую в [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="6b3f0-123">The CLI can be [installed on your local computer](/cli/azure/install-azure-cli) or run directly from the [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

```azurecli
# --------------
# TODO: update the following values
#sets the name of the resource group
resourcegroup=rg-graphevents-dev
#sets the location of the resources
location='uk south'
#sets the name of the Azure Event Hubs namespace
evhamespacename=evh-graphevents-dev
#sets the name of the hub under the namespace
evhhubname=graphevents
#sets the name of the access policy to the hub
evhpolicyname=grapheventspolicy
#sets the name of the Azure KeyVault
keyvaultname=kv-graphevents
#sets the name of the secret in Azure KeyVault that will contain the connection string to the hub
keyvaultsecretname=grapheventsconnectionstring
# --------------
az group create --location $location --name $resourcegroup
az eventhubs namespace create --name $evhamespacename --resource-group $resourcegroup --sku Basic --location $location
az eventhubs eventhub create --name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --partition-count 2 --message-retention 1
az eventhubs eventhub authorization-rule create --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --rights Send
evhprimaryconnectionstring=`az eventhubs eventhub authorization-rule keys list --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --query "primaryConnectionString" --output tsv`
az keyvault create --name $keyvaultname --resource-group $resourcegroup --location $location --enable-soft-delete true --sku standard --retention-days 90
az keyvault secret set --name $keyvaultsecretname --value $evhprimaryconnectionstring --vault-name $keyvaultname --output none
graphspn=`az ad sp list --display-name 'Microsoft Graph Change Tracking' --query "[].appId" --output tsv`
az keyvault set-policy --name $keyvaultname --resource-group $resourcegroup --secret-permissions get --spn $graphspn --output none
keyvaulturi=`az keyvault show --name $keyvaultname --resource-group $resourcegroup --query "properties.vaultUri" --output tsv`
domainname=`az ad signed-in-user show --query 'userPrincipalName' | cut -d '@' -f 2 | sed 's/\"//'`
notificationUrl="EventHub:${keyvaulturi}secrets/${keyvaultsecretname}?tenantId=${domainname}"
echo "Notification Url:\n${notificationUrl}"
```

> <span data-ttu-id="6b3f0-124">**Примечание**. Представленный здесь сценарий совместим с оболочками на основе Linux, Windows WSL и Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-124">**Note:** The script provided here is compatible with Linux based shells, Windows WSL, and Azure Cloud Shell.</span></span> <span data-ttu-id="6b3f0-125">При этом для запуска в оболочках Windows необходимо сделать несколько обновлений.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-125">It will require some updates to run in Windows shells.</span></span>

#### <a name="option-2-using-the-azure-portal"></a><span data-ttu-id="6b3f0-126">Вариант2: использование портала Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f0-126">Option 2: Using the Azure Portal</span></span>

##### <a name="configuring-the-azure-event-hub"></a><span data-ttu-id="6b3f0-127">Настройка концентратора событий Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f0-127">Configuring the Azure Event Hub</span></span>

<span data-ttu-id="6b3f0-128">В этом разделе вы сделаете следующее:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-128">In this section you will:</span></span>

- <span data-ttu-id="6b3f0-129">Создадите пространство имен концентратора событий Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-129">Create an Azure Event Hub namespace.</span></span>
- <span data-ttu-id="6b3f0-130">Добавите в это пространство имен концентратор, который будет пересылать и доставлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-130">Add a hub to that namespace that will relay and deliver notifications.</span></span>
- <span data-ttu-id="6b3f0-131">Добавите политику общего доступа, которая позволит получить строку подключения к только что созданному концентратору.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-131">Add a shared access policy that will allow you to get a connection string to the newly created hub.</span></span>

<span data-ttu-id="6b3f0-132">Шаги:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-132">Steps:</span></span>

1. <span data-ttu-id="6b3f0-133">Откройте [портал Azure](https://portal.azure.com) в браузере.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-133">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="6b3f0-134">Выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-134">Select **Create a resource**.</span></span>
1. <span data-ttu-id="6b3f0-135">В строке поиска введите **концентраторы событий**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-135">Type **Event Hubs** in the search bar.</span></span>
1. <span data-ttu-id="6b3f0-136">Выберите **концентраторы событий** из предложенных.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-136">Select the **Event Hubs** suggestion.</span></span> <span data-ttu-id="6b3f0-137">Будет загружена страница создания концентраторов событий.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-137">The Event Hubs creation page will load.</span></span>  
1. <span data-ttu-id="6b3f0-138">На странице создания концентраторов событий нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-138">On the Event Hubs creation page, click **Create**.</span></span>
1. <span data-ttu-id="6b3f0-139">Заполните сведения о создании пространства имен концентраторов событий и выберите **Cоздать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-139">Fill in the Event Hubs namespace creation details, and then click **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-140">Если пространство имен концентратора событий подготовлено, перейдите к странице пространства имен.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-140">When the Event Hub namespace is provisioned, go to the page for the namespace.</span></span>  
1. <span data-ttu-id="6b3f0-141">Щелкните **Концентраторы событий** и **+ Концентратор событий**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-141">Click **Event Hubs** and **+ Event Hub**.</span></span>  
1. <span data-ttu-id="6b3f0-142">Введите имя нового концентратора событий и щелкните **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-142">Give a name to the new Event Hub, and click **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-143">После того как концентратор событий создан, щелкните на его имя, затем **Политики общего доступа**, а затем **+ Добавить**, чтобы добавить новую политику.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-143">After the Event Hub has been created, click the name of the Event Hub, and then click **Shared access policies** and **+ Add** to add a new policy.</span></span>  
1. <span data-ttu-id="6b3f0-144">Введите имя политики, установите флажок **Отправить** и нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-144">Give a name to the policy, check **Send**, and click **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-145">Когда политика создана, щелкните на ее имя, чтобы открыть область сведений, и скопируйте значение **Первичный ключ строки подключения**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-145">After the policy has been created, click the name of the policy to open the details panel, and then copy the **Connection string-primary key** value.</span></span> <span data-ttu-id="6b3f0-146">Запишите его, так как он понадобится в следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-146">Write it down; you'll need it for the next step.</span></span>  

##### <a name="configuring-the-azure-key-vault"></a><span data-ttu-id="6b3f0-147">Настройка хранилища Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="6b3f0-147">Configuring the Azure Key Vault</span></span>

<span data-ttu-id="6b3f0-148">Для безопасного доступа к концентратору событий и обеспечения ротации ключей Microsoft Graph отправляет строку подключения в концентратор событий через хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-148">In order to access the Event Hub securely and to allow for key rotations, Microsoft Graph gets the connection string to the Event Hub through Azure Key Vault.</span></span>  
<span data-ttu-id="6b3f0-149">В этом разделе вы сделаете следующее:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-149">In this section, you will:</span></span>

- <span data-ttu-id="6b3f0-150">Создадите хранилище Azure Key Vault для хранения секрета.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-150">Create an Azure Key Vault to store secret.</span></span>
- <span data-ttu-id="6b3f0-151">Добавьте строку подключения в качестве секрета в концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-151">Add the connection string to the Event Hub as a secret.</span></span>
- <span data-ttu-id="6b3f0-152">Чтобы получить доступ к секрету, добавьте политику доступа для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-152">Add an access policy for Microsoft Graph to access the secret.</span></span>

<span data-ttu-id="6b3f0-153">Шаги:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-153">Steps:</span></span>

1. <span data-ttu-id="6b3f0-154">Откройте [портал Azure](https://portal.azure.com) в браузере.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-154">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="6b3f0-155">Выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-155">Select **Create a resource**.</span></span>
1. <span data-ttu-id="6b3f0-156">В строке поиска введите **Хранилище ключей**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-156">Type **Key Vault** in the search bar.</span></span>
1. <span data-ttu-id="6b3f0-157">Выберите **хранилище ключей** из предложенных.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-157">Select the **Key Vault** suggestion.</span></span> <span data-ttu-id="6b3f0-158">Будет загружена страница создания хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-158">The Key Vault creation page will load.</span></span>
1. <span data-ttu-id="6b3f0-159">На странице создания хранилища ключей нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-159">On the Key Vault creation page, click **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-160">Заполните сведения для создания хранилища ключей и щелкните **Проверка + создание**, затем **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-160">Fill in the Key Vault creation details, and then click **Review + Create** and **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-161">Перейдите к только что созданному хранилищу, выбрав **Перейти к ресурсу** в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-161">Go to the newly crated key vault using the **Go to resource** from the notification.</span></span>  
1. <span data-ttu-id="6b3f0-162">Скопируйте **DNS-имя**. Это потребуется для следующего шага.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-162">Copy the **DNS name**; you will need it for the next step.</span></span>  
1. <span data-ttu-id="6b3f0-163">Перейдите в **Секреты** и выберите **+ Создать/импортировать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-163">Go to **Secrets** and click **+ Generate/Import**.</span></span>  
1. <span data-ttu-id="6b3f0-164">Введите название секрета и сохраните его для следующего этапа.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-164">Give a name to the secret, and keep the name for later; you will need it for the next step.</span></span> <span data-ttu-id="6b3f0-165">В качестве значения используйте строку подключения, созданную на этапе для концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-165">For the value, paste in the connection string you generated at the Event Hubs step.</span></span> <span data-ttu-id="6b3f0-166">Нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-166">Click **Create**.</span></span>  
1. <span data-ttu-id="6b3f0-167">Щелкните **Политики доступа**, затем **+ Добавить политику доступа**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-167">Click **Access Policies** and **+ Add Access Policy**.</span></span>  
1. <span data-ttu-id="6b3f0-168">Чтобы открыть **Разрешения секретов**, выберите **Получить**, затем **Выбрать первичный**, а затем **Отслеживание изменений в Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-168">For **Secret permissions**, select **Get**, and for **Select Principal**, select **Microsoft Graph Change Tracking**.</span></span> <span data-ttu-id="6b3f0-169">Нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-169">Click **Add**.</span></span>  

### <a name="creating-the-subscription-and-receiving-notifications"></a><span data-ttu-id="6b3f0-170">Создание подписки и просмотр уведомлений</span><span class="sxs-lookup"><span data-stu-id="6b3f0-170">Creating the subscription and receiving notifications</span></span>

<span data-ttu-id="6b3f0-171">После создания обязательных служб хранилища Azure Key Vault и концентраторов событий Azure вы сможете создать свою подписку и начать получать уведомления об изменениях через концентраторы событий Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-171">After you create the required Azure KeyVault and Azure Event Hubs services, you will be able to create your subscription and start receiving change notifications via Azure Event Hubs.</span></span>

#### <a name="creating-the-subcription"></a><span data-ttu-id="6b3f0-172">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="6b3f0-172">Creating the subcription</span></span>

<span data-ttu-id="6b3f0-173">Подписки на изменение уведомлений с помощью концентраторов событий почти идентичны уведомлениям об изменениях с помощью веб-перехватчиков.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-173">Subscriptions to change notifications with Event Hubs are almost identical to change notifications with webhooks.</span></span> <span data-ttu-id="6b3f0-174">Основное отличие заключается в том, что для доставки уведомлений используют концентраторы событий.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-174">The key difference is that they rely on Event Hubs to deliver notifications.</span></span> <span data-ttu-id="6b3f0-175">Другие операции сходны, в том числе [создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6b3f0-175">All other operations are similar, including [subscription creation](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span>  

<span data-ttu-id="6b3f0-176">Основное отличие в ходе создания подписки будет заключаться в значении **notificationUrl,**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-176">The main difference during subscription creation will be the **notificationUrl**.</span></span> <span data-ttu-id="6b3f0-177">Необходимо настроить его на `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>` со следующими значениями:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-177">You must set it to `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`, with the following values:</span></span>

- <span data-ttu-id="6b3f0-178">`azurekeyvaultname` — название созданного хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-178">`azurekeyvaultname` - The name you gave to the key vault when you created it.</span></span> <span data-ttu-id="6b3f0-179">Его можно найти в DNS-имени.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-179">Can be found in the DNS name.</span></span>
- <span data-ttu-id="6b3f0-180">`secretname` — название созданного секрета.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-180">`secretname` - The name you gave to the secret when you created it.</span></span> <span data-ttu-id="6b3f0-181">Его можно найти на странице **Секреты** в хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-181">Can be found on the Azure Key Vault **Secrets** page.</span></span>
- <span data-ttu-id="6b3f0-182">`domainname` — имя клиента, например, consto.onmicrosoft.com или contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-182">`domainname` - The name of your tenant; for example, consto.onmicrosoft.com or contoso.com.</span></span> <span data-ttu-id="6b3f0-183">Поскольку этот домен будет использоваться для доступа к хранилищу Azure Key Vault, важно, чтобы он соответствовал домену, используемому подпиской Azure с хранилищем Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-183">Because this domain will be used to access the Azure Key Vault, it is important that it matches the domain used by the Azure subscription that holds the Azure Key Vault.</span></span> <span data-ttu-id="6b3f0-184">Чтобы получить эту информацию, вы можете перейти на страницу обзора созданного хранилища Azure Key Vault и щелкнуть на подписку.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-184">To get this information, you can go to the overview page of the Azure Key Vault you created and click the subscription.</span></span> <span data-ttu-id="6b3f0-185">Имя домена выводится в поле **Каталог**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-185">The domain name is displayed under the **Directory** field.</span></span>

#### <a name="receiving-notifications"></a><span data-ttu-id="6b3f0-186">Получение уведомлений</span><span class="sxs-lookup"><span data-stu-id="6b3f0-186">Receiving notifications</span></span>

<span data-ttu-id="6b3f0-187">События будут доставлены концентраторами событий в ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-187">Events will be now delivered to your application by Event Hubs.</span></span> <span data-ttu-id="6b3f0-188">Дополнительные сведения см. в статье [Получение событий](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) в документации по концентраторам событий.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-188">For details, see [receiving events](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) in the Event Hubs documentation.</span></span>

<span data-ttu-id="6b3f0-189">Чтобы вы могли получать уведомления в приложении, потребуется создать еще одну политику общего доступа с разрешением на "Прослушивание" и получить строку подключения, как в инструкциях из раздела [Настройка концентратора событий Azure](#configuring-the-azure-event-hub).</span><span class="sxs-lookup"><span data-stu-id="6b3f0-189">Before you can receive the notifications in your application, you'll need to create another shared access policy with a "Listen" permission and obtain the connection string, similar to the steps listed in [Configuring the Azure Event Hub](#configuring-the-azure-event-hub).</span></span>

> <span data-ttu-id="6b3f0-190">**Примечание**. Создайте отдельную политику для приложения, которое прослушивает сообщения в концентраторах событий, вместо того чтобы повторно использовать строку подключения, заданную в хранилище Azure KeyVault.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-190">**Note:** Create a separate policy for the application that listens to Event Hubs messages instead of reusing the same connection string you set in Azure KeyVault.</span></span> <span data-ttu-id="6b3f0-191">Это гарантирует, что каждый компонент решения будет иметь только нужные разрешения в соответствии с принципом минимальных разрешений.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-191">This ensures that each component of the solution has only the permissions it needs and follows the least permissions security principle.</span></span>

> <span data-ttu-id="6b3f0-192">**Примечание.** Ваше приложение будет получать сообщения о проверке каждый раз при создании новой подписки.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-192">**Note:** Your application receives validation messages whenever it creates a new subscription.</span></span> <span data-ttu-id="6b3f0-193">Эти уведомления следует пропустить.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-193">You should ignore these notifications.</span></span> <span data-ttu-id="6b3f0-194">В приведенном ниже примере представлен текст сообщения о проверке.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-194">The following example represents the body of a validation message.</span></span>

```json
 {
    "value":[
        {
            "subscriptionId":"NA",
            "subscriptionExpirationDateTime":"NA",
            "clientState":"NA",
            "changeType":"Validation: Testing client application reachability for subscription Request-Id: 522a8e7e-096a-494c-aaf1-ac0dcfca45b7",
            "resource":"NA",
            "resourceData":{
                "@odata.type":"NA",
                "@odata.id":"NA",
                "id":"NA"
            }
        }
    ]
}
```

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a><span data-ttu-id="6b3f0-195">Что произойдет, если приложение для отслеживания изменений в Microsoft Graph отсутствует?</span><span class="sxs-lookup"><span data-stu-id="6b3f0-195">What happens if the Microsoft Graph change tracking application is missing?</span></span>

<span data-ttu-id="6b3f0-196">Возможно, в вашем клиенте нет субъекта-службы **отслеживания изменений в Microsoft Graph**. Это зависит от того, когда был создан клиент и от административных операций.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-196">It's possible that the **Microsoft Graph Change Tracking** service principal is missing from your tenant, depending on when the tenant was created and administrative operations.</span></span> <span data-ttu-id="6b3f0-197">Чтобы устранить эту проблему, выполните [следующий запрос](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) в [проводнике Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6b3f0-197">To resolve this issue, run [the following query](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) in [Microsoft Graph Explorer](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span></span>

<span data-ttu-id="6b3f0-198">Подробности запроса:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-198">Query details:</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> <span data-ttu-id="6b3f0-199">**Примечание.** Вы можете получить отказ в выполнении этого запроса.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-199">**Note:** You can get an access denied running this query.</span></span> <span data-ttu-id="6b3f0-200">В этом случае щелкните значок шестеренки рядом с именем своей учетной записи в левом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-200">In this case, select the gear icon next to your account name in the top left corner.</span></span> <span data-ttu-id="6b3f0-201">Затем выберите **Выбрать разрешения**, а затем выполните поиск по запросу **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-201">Then select **Select Permissions** and search for **Application.ReadWrite.All**.</span></span> <span data-ttu-id="6b3f0-202">Проверьте разрешения и выберите **Согласие**.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-202">Check the permission and select **Consent**.</span></span> <span data-ttu-id="6b3f0-203">После того как вы подтвердите новое разрешение, снова выполните поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-203">After consenting to this new permission, run the request again.</span></span>

> <span data-ttu-id="6b3f0-204">**Примечание.** Этот API-интерфейс действует только для учебной или рабочей учетной записи, но не в личной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-204">**Note:** This API only works with a school or work account, not with a personal account.</span></span> <span data-ttu-id="6b3f0-205">Убедитесь, что вы вошли в систему через учетную запись в своем домене.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-205">Make sure that you are signed in with an account on your domain.</span></span>

<span data-ttu-id="6b3f0-206">Кроме того, вы можете использовать данный сценарий [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0), чтобы добавлять недостающие субъекты-службы.</span><span class="sxs-lookup"><span data-stu-id="6b3f0-206">Alternatively, you can use this [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) script to add the missing service principal.</span></span>

```PowerShell
Connect-AzureAD -TenantId <tenant-id>
# replace tenant-id by the id of your tenant.
New-AzureADServicePrincipal -AppId 0bf30f3b-4a52-48df-9a82-234910c4a086
```

## <a name="next-steps"></a><span data-ttu-id="6b3f0-207">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6b3f0-207">Next steps</span></span>

<span data-ttu-id="6b3f0-208">См. следующие краткие руководства о концентраторах событий Azure:</span><span class="sxs-lookup"><span data-stu-id="6b3f0-208">See the following Azure Event Hubs quick starts:</span></span>

- [<span data-ttu-id="6b3f0-209">.NET Core</span><span class="sxs-lookup"><span data-stu-id="6b3f0-209">.NET Core</span></span>](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [<span data-ttu-id="6b3f0-210">Java</span><span class="sxs-lookup"><span data-stu-id="6b3f0-210">Java</span></span>](/azure/event-hubs/event-hubs-java-get-started-send)
- [<span data-ttu-id="6b3f0-211">Python</span><span class="sxs-lookup"><span data-stu-id="6b3f0-211">Python</span></span>](/azure/event-hubs/get-started-python-send-v2)
- [<span data-ttu-id="6b3f0-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b3f0-212">JavaScript</span></span>](/azure/event-hubs/get-started-node-send-v2)
