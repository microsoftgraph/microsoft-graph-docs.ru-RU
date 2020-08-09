---
title: Получение уведомлений об изменениях разными способами (предварительная версия)
description: Уведомления об изменениях можно получать с помощью разных технологий, включая веб-перехватчики и концентраторы событий Azure.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 83014782c98d0807681a9d8da0d37b6092df167b
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598612"
---
# <a name="get-change-notifications-delivered-in-different-ways-preview"></a><span data-ttu-id="2483b-103">Получение уведомлений об изменениях разными способами (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2483b-103">Get change notifications delivered in different ways (preview)</span></span>

<span data-ttu-id="2483b-104">Уведомления об изменениях можно отправлять подписчикам разными способами.</span><span class="sxs-lookup"><span data-stu-id="2483b-104">Change notifications can be delivered in different ways to subscribers.</span></span> <span data-ttu-id="2483b-105">Если основной способ доставки уведомлений об изменениях — веб-перехватчики, может оказаться непросто использовать преимущества веб-перехватчиков в условиях высокой пропускной способности или когда получатель не может предоставить общедоступный URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="2483b-105">If the main delivery mode for change notifications is through webhooks, it can be challenging to take advantage of webhooks for high throughput scenarios or when the receiver cannot expose a publicly available notificiation URL.</span></span>  

<span data-ttu-id="2483b-106">Ниже приведены примеры сценариев с высокой пропускной способностью, в том числе приложения, которые подписаны на многие ресурсы, приложения, которые подписаны на часто изменяющиеся ресурсы, и многоуровневые приложения, которые подписаны на ресурсы в рамках большого набора организаций.</span><span class="sxs-lookup"><span data-stu-id="2483b-106">Good examples of high throughput scenarios include applications subscribing to a large set of resources, applications subscribing to resources that change with a high frequency, and multi-tenant applications that subscribe to resources accross a large set of organizations.</span></span>

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a><span data-ttu-id="2483b-107">Получение уведомлений об изменениях с помощью концентраторов событий Azure</span><span class="sxs-lookup"><span data-stu-id="2483b-107">Using Azure Event Hubs to receive change notifications</span></span>

<span data-ttu-id="2483b-108">[Концентраторы событий Azure](https://azure.microsoft.com/services/event-hubs) — это сервис приема и распространения популярных событий в режиме реального времени, созданный для масштабирования.</span><span class="sxs-lookup"><span data-stu-id="2483b-108">[Azure Event Hubs](https://azure.microsoft.com/services/event-hubs) is a popular real-time events ingestion and distribution service built for scale.</span></span> <span data-ttu-id="2483b-109">Для получения уведомлений об изменениях вместо традиционных веб-перехватчиков можно использовать концентраторы событий Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-109">You can use Azure Events Hubs instead of traditional webhooks to receive change notifications.</span></span> <span data-ttu-id="2483b-110">В настоящее время эта функция находится на стадии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2483b-110">This feature is currently in preview.</span></span>  
<span data-ttu-id="2483b-111">Использование концентраторов событий Azure для получения уведомлений о изменениях отличается от веб-перехватчиков несколькими моментами, в том числе:</span><span class="sxs-lookup"><span data-stu-id="2483b-111">Using Azure Event Hubs to receive change notifications differs from webhooks in a few ways, including:</span></span>

- <span data-ttu-id="2483b-112">Не приходится полагаться на общедоступные URL-адреса уведомлений.</span><span class="sxs-lookup"><span data-stu-id="2483b-112">You don't rely on publicly exposed notification URLs.</span></span> <span data-ttu-id="2483b-113">Пакет SDK концентраторов событий ретранслирует уведомления в ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="2483b-113">The Event Hubs SDK will relay the notifications to your application.</span></span>
- <span data-ttu-id="2483b-114">Не нужно реализовывать [проверку URL-адреса уведомлений](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="2483b-114">You don't need to implement the [notification URL validation](webhooks.md#notification-endpoint-validation).</span></span>
- <span data-ttu-id="2483b-115">Необходимо подготовить концентратор событий Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-115">You'll need to provision an Azure Event Hub.</span></span>
- <span data-ttu-id="2483b-116">Необходимо подготовить хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="2483b-116">You'll need to provision an Azure Key Vault.</span></span>

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a><span data-ttu-id="2483b-117">Настройка хранилища Azure Key Vault и концентраторов событий Azure</span><span class="sxs-lookup"><span data-stu-id="2483b-117">Set up the Azure KeyVault and Azure Event Hubs</span></span>

<span data-ttu-id="2483b-118">В этом разделе вы узнаете, как выполнить настройку обязательных служб Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-118">This section will walk you through the setup of required Azure services.</span></span>

#### <a name="option-1-using-the-azure-cli"></a><span data-ttu-id="2483b-119">Вариант 1: использование CLI</span><span class="sxs-lookup"><span data-stu-id="2483b-119">Option 1: Using the Azure CLI</span></span>

<span data-ttu-id="2483b-120">Средство [Azure CLI](/cli/azure/what-is-azure-cli?view=azure-cli-latest) позволяет создавать сценарии и автоматизировать админстративные задачи в Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-120">The [Azure CLI](/cli/azure/what-is-azure-cli?view=azure-cli-latest) allows you to script and automate adminstrative tasks in Azure.</span></span> <span data-ttu-id="2483b-121">Средство CLI можно [установить на локальный компьютер](/cli/azure/install-azure-cli?view=azure-cli-latest) или запустить напрямую в [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="2483b-121">The CLI can be [installed on your local computer](/cli/azure/install-azure-cli?view=azure-cli-latest) or run directly from the [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

```shell
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

> <span data-ttu-id="2483b-122">**Примечание**. Представленный здесь сценарий совместим с оболочками на основе Linux, Windows WSL и Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2483b-122">**Note:** The script provided here is compatible with Linux based shells, Windows WSL, and Azure Cloud Shell.</span></span> <span data-ttu-id="2483b-123">При этом для запуска в оболочках Windows необходимо сделать несколько обновлений.</span><span class="sxs-lookup"><span data-stu-id="2483b-123">It will require some updates to run in Windows shells.</span></span>

#### <a name="option-2-using-the-azure-portal"></a><span data-ttu-id="2483b-124">Вариант2: использование портала Azure</span><span class="sxs-lookup"><span data-stu-id="2483b-124">Option 2: Using the Azure Portal</span></span>

##### <a name="configuring-the-azure-event-hub"></a><span data-ttu-id="2483b-125">Настройка концентратора событий Azure</span><span class="sxs-lookup"><span data-stu-id="2483b-125">Configuring the Azure Event Hub</span></span>

<span data-ttu-id="2483b-126">В этом разделе вы сделаете следующее:</span><span class="sxs-lookup"><span data-stu-id="2483b-126">In this section you will:</span></span>

- <span data-ttu-id="2483b-127">Создадите пространство имен концентратора событий Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-127">Create an Azure Event Hub namespace.</span></span>
- <span data-ttu-id="2483b-128">Добавите в это пространство имен концентратор, который будет пересылать и доставлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="2483b-128">Add a hub to that namespace that will relay and deliver notifications.</span></span>
- <span data-ttu-id="2483b-129">Добавите политику общего доступа, которая позволит получить строку подключения к только что созданному концентратору.</span><span class="sxs-lookup"><span data-stu-id="2483b-129">Add a shared access policy that will allow you to get a connection string to the newly created hub.</span></span>

<span data-ttu-id="2483b-130">Шаги:</span><span class="sxs-lookup"><span data-stu-id="2483b-130">Steps:</span></span>

1. <span data-ttu-id="2483b-131">Откройте [портал Azure](https://portal.azure.com) в браузере.</span><span class="sxs-lookup"><span data-stu-id="2483b-131">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="2483b-132">Выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="2483b-132">Select **Create a resource**.</span></span>
1. <span data-ttu-id="2483b-133">В строке поиска введите **концентраторы событий**.</span><span class="sxs-lookup"><span data-stu-id="2483b-133">Type **Event Hubs** in the search bar.</span></span>
1. <span data-ttu-id="2483b-134">Выберите **концентраторы событий** из предложенных.</span><span class="sxs-lookup"><span data-stu-id="2483b-134">Select the **Event Hubs** suggestion.</span></span> <span data-ttu-id="2483b-135">Будет загружена страница создания концентраторов событий.</span><span class="sxs-lookup"><span data-stu-id="2483b-135">The Event Hubs creation page will load.</span></span>  
1. <span data-ttu-id="2483b-136">На странице создания концентраторов событий нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-136">On the Event Hubs creation page, click **Create**.</span></span>
1. <span data-ttu-id="2483b-137">Заполните сведения о создании пространства имен концентраторов событий и выберите **Cоздать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-137">Fill in the Event Hubs namespace creation details, and then click **Create**.</span></span>  
1. <span data-ttu-id="2483b-138">Если пространство имен концентратора событий подготовлено, перейдите к странице пространства имен.</span><span class="sxs-lookup"><span data-stu-id="2483b-138">When the Event Hub namespace is provisioned, go to the page for the namespace.</span></span>  
1. <span data-ttu-id="2483b-139">Щелкните **Концентраторы событий** и **+ Концентратор событий**.</span><span class="sxs-lookup"><span data-stu-id="2483b-139">Click **Event Hubs** and **+ Event Hub**.</span></span>  
1. <span data-ttu-id="2483b-140">Введите имя нового концентратора событий и щелкните **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-140">Give a name to the new Event Hub, and click **Create**.</span></span>  
1. <span data-ttu-id="2483b-141">После того как концентратор событий создан, щелкните на его имя, затем **Политики общего доступа**, а затем **+ Добавить**, чтобы добавить новую политику.</span><span class="sxs-lookup"><span data-stu-id="2483b-141">After the Event Hub has been created, click the name of the Event Hub, and then click **Shared access policies** and **+ Add** to add a new policy.</span></span>  
1. <span data-ttu-id="2483b-142">Введите имя политики, установите флажок **Отправить**и нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-142">Give a name to the policy, check **Send**, and click **Create**.</span></span>  
1. <span data-ttu-id="2483b-143">Когда политика создана, щелкните на ее имя, чтобы открыть область сведений, и скопируйте значение **Первичный ключ строки подключения**.</span><span class="sxs-lookup"><span data-stu-id="2483b-143">After the policy has been created, click the name of the policy to open the details panel, and then copy the **Connection string-primary key** value.</span></span> <span data-ttu-id="2483b-144">Запишите его, так как он понадобится в следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="2483b-144">Write it down; you'll need it for the next step.</span></span>  

##### <a name="configuring-the-azure-key-vault"></a><span data-ttu-id="2483b-145">Настройка хранилища Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="2483b-145">Configuring the Azure Key Vault</span></span>

<span data-ttu-id="2483b-146">Для безопасного доступа к концентратору событий и обеспечения ротации ключей Microsoft Graph отправляет строку подключения в концентратор событий через хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="2483b-146">In order to access the Event Hub securely and to allow for key rotations, Microsoft Graph gets the connection string to the Event Hub through Azure Key Vault.</span></span>  
<span data-ttu-id="2483b-147">В этом разделе вы сделаете следующее:</span><span class="sxs-lookup"><span data-stu-id="2483b-147">In this section, you will:</span></span>

- <span data-ttu-id="2483b-148">Создадите хранилище Azure Key Vault для хранения секрета.</span><span class="sxs-lookup"><span data-stu-id="2483b-148">Create an Azure Key Vault to store secret.</span></span>
- <span data-ttu-id="2483b-149">Добавьте строку подключения в качестве секрета в концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="2483b-149">Add the connection string to the Event Hub as a secret.</span></span>
- <span data-ttu-id="2483b-150">Чтобы получить доступ к секрету, добавьте политику доступа для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2483b-150">Add an access policy for Microsoft Graph to access the secret.</span></span>

<span data-ttu-id="2483b-151">Шаги:</span><span class="sxs-lookup"><span data-stu-id="2483b-151">Steps:</span></span>

1. <span data-ttu-id="2483b-152">Откройте [портал Azure](https://portal.azure.com) в браузере.</span><span class="sxs-lookup"><span data-stu-id="2483b-152">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="2483b-153">Выберите **Создать ресурс**.</span><span class="sxs-lookup"><span data-stu-id="2483b-153">Select **Create a resource**.</span></span>
1. <span data-ttu-id="2483b-154">В строке поиска введите **Хранилище ключей**.</span><span class="sxs-lookup"><span data-stu-id="2483b-154">Type **Key Vault** in the search bar.</span></span>
1. <span data-ttu-id="2483b-155">Выберите **хранилище ключей** из предложенных.</span><span class="sxs-lookup"><span data-stu-id="2483b-155">Select the **Key Vault** suggestion.</span></span> <span data-ttu-id="2483b-156">Будет загружена страница создания хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="2483b-156">The Key Vault creation page will load.</span></span>
1. <span data-ttu-id="2483b-157">На странице создания хранилища ключей нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-157">On the Key Vault creation page, click **Create**.</span></span>  
1. <span data-ttu-id="2483b-158">Заполните сведения для создания хранилища ключей и щелкните **Проверка + создание**, затем **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-158">Fill in the Key Vault creation details, and then click **Review + Create** and **Create**.</span></span>  
1. <span data-ttu-id="2483b-159">Перейдите к только что созданному хранилищу, выбрав **Перейти к ресурсу** в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="2483b-159">Go to the newly crated key vault using the **Go to resource** from the notification.</span></span>  
1. <span data-ttu-id="2483b-160">Скопируйте **DNS-имя**. Это потребуется для следующего шага.</span><span class="sxs-lookup"><span data-stu-id="2483b-160">Copy the **DNS name**; you will need it for the next step.</span></span>  
1. <span data-ttu-id="2483b-161">Перейдите в **Секреты** и выберите **+ Создать/импортировать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-161">Go to **Secrets** and click **+ Generate/Import**.</span></span>  
1. <span data-ttu-id="2483b-162">Введите название секрета и сохраните его для следующего этапа.</span><span class="sxs-lookup"><span data-stu-id="2483b-162">Give a name to the secret, and keep the name for later; you will need it for the next step.</span></span> <span data-ttu-id="2483b-163">В качестве значения используйте строку подключения, созданную на этапе для концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="2483b-163">For the value, paste in the connection string you generated at the Event Hubs step.</span></span> <span data-ttu-id="2483b-164">Нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2483b-164">Click **Create**.</span></span>  
1. <span data-ttu-id="2483b-165">Щелкните **Политики доступа**, затем **+ Добавить политику доступа**.</span><span class="sxs-lookup"><span data-stu-id="2483b-165">Click **Access Policies** and **+ Add Access Policy**.</span></span>  
1. <span data-ttu-id="2483b-166">Чтобы открыть **Разрешения секретов**, выберите **Получить**, затем **Выбрать первичный**, а затем **Отслеживание изменений в Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="2483b-166">For **Secret permissions**, select **Get**, and for **Select Principal**, select **Microsoft Graph Change Tracking**.</span></span> <span data-ttu-id="2483b-167">Нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="2483b-167">Click **Add**.</span></span>  

### <a name="creating-the-subscription-and-receiving-notifications"></a><span data-ttu-id="2483b-168">Создание подписки и просмотр уведомлений</span><span class="sxs-lookup"><span data-stu-id="2483b-168">Creating the subscription and receiving notifications</span></span>

<span data-ttu-id="2483b-169">После создания обязательных служб хранилища Azure Key Vault и концентраторов событий Azure вы сможете создать свою подписку и начать получать уведомления об изменениях через концентраторы событий Azure.</span><span class="sxs-lookup"><span data-stu-id="2483b-169">After you create the required Azure KeyVault and Azure Event Hubs services, you will be able to create your subscription and start receiving change notifications via Azure Event Hubs.</span></span>

#### <a name="creating-the-subcription"></a><span data-ttu-id="2483b-170">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2483b-170">Creating the subcription</span></span>

<span data-ttu-id="2483b-171">Подписки на изменение уведомлений с помощью концентраторов событий почти идентичны уведомлениям об изменениях с помощью веб-перехватчиков.</span><span class="sxs-lookup"><span data-stu-id="2483b-171">Subscriptions to change notifications with Event Hubs are almost identical to change notifications with webhooks.</span></span> <span data-ttu-id="2483b-172">Основное отличие заключается в том, что для доставки уведомлений используют концентраторы событий.</span><span class="sxs-lookup"><span data-stu-id="2483b-172">The key difference is that they rely on Event Hubs to deliver notifications.</span></span> <span data-ttu-id="2483b-173">Другие операции сходны, в том числе [создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="2483b-173">All other operations are similar, including [subscription creation](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span>  

<span data-ttu-id="2483b-174">Основное отличие в ходе создания подписки будет заключаться в значении **notificationUrl,**.</span><span class="sxs-lookup"><span data-stu-id="2483b-174">The main difference during subscription creation will be the **notificationUrl**.</span></span> <span data-ttu-id="2483b-175">Необходимо настроить его на `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>` со следующими значениями:</span><span class="sxs-lookup"><span data-stu-id="2483b-175">You must set it to `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`, with the following values:</span></span>

- <span data-ttu-id="2483b-176">`azurekeyvaultname` — название созданного хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="2483b-176">`azurekeyvaultname` - The name you gave to the key vault when you created it.</span></span> <span data-ttu-id="2483b-177">Его можно найти в DNS-имени.</span><span class="sxs-lookup"><span data-stu-id="2483b-177">Can be found in the DNS name.</span></span>
- <span data-ttu-id="2483b-178">`secretname` — название созданного секрета.</span><span class="sxs-lookup"><span data-stu-id="2483b-178">`secretname` - The name you gave to the secret when you created it.</span></span> <span data-ttu-id="2483b-179">Его можно найти на странице **Секреты** в хранилище Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="2483b-179">Can be found on the Azure Key Vault **Secrets** page.</span></span>
- <span data-ttu-id="2483b-180">`domainname` — имя клиента, например, consto.onmicrosoft.com или contoso.com.</span><span class="sxs-lookup"><span data-stu-id="2483b-180">`domainname` - The name of your tenant; for example, consto.onmicrosoft.com or contoso.com.</span></span> <span data-ttu-id="2483b-181">Поскольку этот домен будет использоваться для доступа к хранилищу Azure Key Vault, важно, чтобы он соответствовал домену, используемому подпиской Azure с хранилищем Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="2483b-181">Because this domain will be used to access the Azure Key Vault, it is important that it matches the domain used by the Azure subscription that holds the Azure Key Vault.</span></span> <span data-ttu-id="2483b-182">Чтобы получить эту информацию, вы можете перейти на страницу обзора созданного хранилища Azure Key Vault и щелкнуть на подписку.</span><span class="sxs-lookup"><span data-stu-id="2483b-182">To get this information, you can go to the overview page of the Azure Key Vault you created and click the subscription.</span></span> <span data-ttu-id="2483b-183">Имя домена выводится в поле **Каталог**.</span><span class="sxs-lookup"><span data-stu-id="2483b-183">The domain name is displayed under the **Directory** field.</span></span>

#### <a name="receiving-notifications"></a><span data-ttu-id="2483b-184">Получение уведомлений</span><span class="sxs-lookup"><span data-stu-id="2483b-184">Receiving notifications</span></span>

<span data-ttu-id="2483b-185">События будут доставлены концентраторами событий в ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="2483b-185">Events will be now delivered to your application by Event Hubs.</span></span> <span data-ttu-id="2483b-186">Дополнительные сведения см. в статье [Получение событий](https://docs.microsoft.com/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) в документации по концентраторам событий.</span><span class="sxs-lookup"><span data-stu-id="2483b-186">For details, see [receiving events](https://docs.microsoft.com/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) in the Event Hubs documentation.</span></span>

<span data-ttu-id="2483b-187">Чтобы вы могли получать уведомления в приложении, потребуется создать еще одну политику общего доступа с разрешением на "Прослушивание" и получить строку подключения, как в инструкциях из раздела [Настройка концентратора событий Azure](#configuring-the-azure-event-hub).</span><span class="sxs-lookup"><span data-stu-id="2483b-187">Before you can receive the notifications in your application, you'll need to create another shared access policy with a "Listen" permission and obtain the connection string, similar to the steps listed in [Configuring the Azure Event Hub](#configuring-the-azure-event-hub).</span></span>

> <span data-ttu-id="2483b-188">**Примечание**. Создайте отдельную политику для приложения, которое прослушивает сообщения в концентраторах событий, вместо того чтобы повторно использовать строку подключения, заданную в хранилище Azure KeyVault.</span><span class="sxs-lookup"><span data-stu-id="2483b-188">**Note:** Create a separate policy for the application that listens to Event Hubs messages instead of reusing the same connection string you set in Azure KeyVault.</span></span> <span data-ttu-id="2483b-189">Это гарантирует, что каждый компонент решения будет иметь только нужные разрешения в соответствии с принципом минимальных разрешений.</span><span class="sxs-lookup"><span data-stu-id="2483b-189">This ensures that each component of the solution has only the permissions it needs and follows the least permissions security principle.</span></span>

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a><span data-ttu-id="2483b-190">Что произойдет, если приложение для отслеживания изменений в Microsoft Graph отсутствует?</span><span class="sxs-lookup"><span data-stu-id="2483b-190">What happens if the Microsoft Graph change tracking application is missing?</span></span>

<span data-ttu-id="2483b-191">Возможно, в вашем клиенте нет субъекта-службы **отслеживания изменений в Microsoft Graph**. Это зависит от того, когда был создан клиент и от административных операций.</span><span class="sxs-lookup"><span data-stu-id="2483b-191">It's possible that the **Microsoft Graph Change Tracking** service principal is missing from your tenant, depending on when the tenant was created and administrative operations.</span></span> <span data-ttu-id="2483b-192">Чтобы устранить эту проблему, выполните [следующий запрос](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) в [проводнике Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="2483b-192">To resolve this issue, run [the following query](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) in [Microsoft Graph Explorer](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span></span>

<span data-ttu-id="2483b-193">Подробности запроса:</span><span class="sxs-lookup"><span data-stu-id="2483b-193">Query details:</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> <span data-ttu-id="2483b-194">**Примечание.** Вы можете получить отказ в выполнении этого запроса.</span><span class="sxs-lookup"><span data-stu-id="2483b-194">**Note:** You can get an access denied running this query.</span></span> <span data-ttu-id="2483b-195">В этом случае щелкните значок шестеренки рядом с именем своей учетной записи в левом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="2483b-195">In this case, select the gear icon next to your account name in the top left corner.</span></span> <span data-ttu-id="2483b-196">Затем выберите **Выбрать разрешения**, а затем выполните поиск по запросу **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="2483b-196">Then select **Select Permissions** and search for **Application.ReadWrite.All**.</span></span> <span data-ttu-id="2483b-197">Проверьте разрешения и выберите **Согласие**.</span><span class="sxs-lookup"><span data-stu-id="2483b-197">Check the permission and select **Consent**.</span></span> <span data-ttu-id="2483b-198">После того как вы подтвердите новое разрешение, снова выполните поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="2483b-198">After consenting to this new permission, run the request again.</span></span>

> <span data-ttu-id="2483b-199">**Примечание.** Этот API-интерфейс действует только для учебной или рабочей учетной записи, но не в личной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2483b-199">**Note:** This API only works with a school or work account, not with a personal account.</span></span> <span data-ttu-id="2483b-200">Убедитесь, что вы вошли в систему через учетную запись в своем домене.</span><span class="sxs-lookup"><span data-stu-id="2483b-200">Make sure that you are signed in with an account on your domain.</span></span>

<span data-ttu-id="2483b-201">Кроме того, вы можете использовать данный сценарий [Azure Active Directory PowerShell](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0), чтобы добавлять недостающие субъекты-службы.</span><span class="sxs-lookup"><span data-stu-id="2483b-201">Alternatively, you can use this [Azure Active Directory PowerShell](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) script to add the missing service principal.</span></span>

```PowerShell
Connect-AzureAD -TenantId <tenant-id>
# replace tenant-id by the id of your tenant.
New-AzureADServicePrincipal -AppId 0bf30f3b-4a52-48df-9a82-234910c4a086
```

## <a name="next-steps"></a><span data-ttu-id="2483b-202">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2483b-202">Next steps</span></span>

<span data-ttu-id="2483b-203">См. следующие краткие руководства о концентраторах событий Azure:</span><span class="sxs-lookup"><span data-stu-id="2483b-203">See the following Azure Event Hubs quick starts:</span></span>

- [<span data-ttu-id="2483b-204">.NET Core</span><span class="sxs-lookup"><span data-stu-id="2483b-204">.NET Core</span></span>](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [<span data-ttu-id="2483b-205">Java</span><span class="sxs-lookup"><span data-stu-id="2483b-205">Java</span></span>](/azure/event-hubs/event-hubs-java-get-started-send)
- [<span data-ttu-id="2483b-206">Python</span><span class="sxs-lookup"><span data-stu-id="2483b-206">Python</span></span>](/azure/event-hubs/get-started-python-send-v2)
- [<span data-ttu-id="2483b-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2483b-207">JavaScript</span></span>](/azure/event-hubs/get-started-node-send-v2)
