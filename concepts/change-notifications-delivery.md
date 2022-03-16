---
title: Получение уведомлений об изменениях разными способами
description: Уведомления об изменениях можно получать с помощью разных технологий, включая веб-перехватчики и концентраторы событий Azure.
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 5a93ed69c7e0ed83dcb9ac9d877a59b9033d30b2
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500905"
---
# <a name="get-change-notifications-delivered-in-different-ways"></a>Получение уведомлений об изменениях разными способами

Пользователи могут получать уведомления об изменениях разными способами. Если основной способ доставки уведомлений об изменениях — веб-перехватчики, может оказаться непросто использовать их преимущества в условиях высокой пропускной способности или когда получатель не может предоставить общедоступный URL-адрес уведомлений.  

Этот способ доставки уведомлений об изменениях доступен для всех ресурсов, поддерживающих уведомления об изменениях Microsoft Graph.

Ниже приведены примеры сценариев с высокой пропускной способностью, в том числе приложения, которые подписаны на многие ресурсы, приложения, которые подписаны на часто изменяющиеся ресурсы, и многоуровневые приложения, которые подписаны на ресурсы в рамках большого набора организаций.

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a>Получение уведомлений об изменениях с помощью концентраторов событий Azure

[Концентраторы событий Azure](https://azure.microsoft.com/services/event-hubs) — это сервис приема и распространения популярных событий в режиме реального времени, созданный для масштабирования. Для получения уведомлений об изменениях вместо традиционных веб-перехватчиков можно использовать концентраторы событий Azure.  
Использование концентраторов событий Azure для получения уведомлений о изменениях отличается от веб-перехватчиков несколькими моментами, в том числе:

- Не приходится полагаться на общедоступные URL-адреса уведомлений. Пакет SDK концентраторов событий ретранслирует уведомления в ваше приложение.
- Нет необходимости отвечать на [проверку URL-адреса уведомлений](webhooks.md#notification-endpoint-validation). Можно пропустить полученное сообщение о проверке.
- Необходимо подготовить концентратор событий Azure.
- Необходимо подготовить хранилище Azure Key Vault.

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a>Настройка хранилища Azure Key Vault и концентраторов событий Azure

В этом разделе вы узнаете, как выполнить настройку обязательных служб Azure.

#### <a name="option-1-using-the-azure-cli"></a>Вариант 1: использование CLI

Средство [Azure CLI](/cli/azure/what-is-azure-cli) позволяет создавать сценарии и автоматизировать админстративные задачи в Azure. Средство CLI можно [установить на локальный компьютер](/cli/azure/install-azure-cli) или запустить напрямую в [Azure Cloud Shell](/azure/cloud-shell/quickstart).

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

> **Примечание**. Представленный здесь сценарий совместим с оболочками на основе Linux, Windows WSL и Azure Cloud Shell. При этом для запуска в оболочках Windows необходимо сделать несколько обновлений.

#### <a name="option-2-using-the-azure-portal"></a>Вариант2: использование портала Azure

##### <a name="configuring-the-azure-event-hub"></a>Настройка концентратора событий Azure

В этом разделе вы сделаете следующее:

- Создадите пространство имен концентратора событий Azure.
- Добавите в это пространство имен концентратор, который будет пересылать и доставлять уведомления.
- Добавите политику общего доступа, которая позволит получить строку подключения к только что созданному концентратору.

Шаги:

1. Откройте [портал Azure](https://portal.azure.com) в браузере.
1. Выберите **Создать ресурс**.
1. В строке поиска введите **концентраторы событий**.
1. Выберите **концентраторы событий** из предложенных. Будет загружена страница создания концентраторов событий.  
1. На странице создания концентраторов событий нажмите **Создать**.
1. Заполните сведения о создании пространства имен концентраторов событий и выберите **Cоздать**.  
1. Если пространство имен концентратора событий подготовлено, перейдите к странице пространства имен.  
1. Щелкните **Концентраторы событий** и **+ Концентратор событий**.  
1. Введите имя нового концентратора событий и щелкните **Создать**.  
1. После того как концентратор событий создан, щелкните на его имя, затем **Политики общего доступа**, а затем **+ Добавить**, чтобы добавить новую политику.  
1. Введите имя политики, установите флажок **Отправить** и нажмите **Создать**.  
1. Когда политика будет создана, щелкните ее имя, чтобы открыть панель сведений, и скопируйте значение **Первичный ключ строки подключения**. Запишите его, так как он понадобится на следующем шаге.  

##### <a name="configuring-the-azure-key-vault"></a>Настройка хранилища Azure Key Vault

Для безопасного доступа к концентратору событий и обеспечения ротации ключей Microsoft Graph отправляет строку подключения в концентратор событий через хранилище Azure Key Vault.  
В этом разделе вы сделаете следующее:

- Создадите хранилище Azure Key Vault для хранения секрета.
- Добавьте строку подключения в качестве секрета в концентратор событий.
- Чтобы получить доступ к секрету, добавьте политику доступа для Microsoft Graph.

Шаги:

1. Откройте [портал Azure](https://portal.azure.com) в браузере.
1. Выберите **Создать ресурс**.
1. В строке поиска введите **Хранилище ключей**.
1. Выберите **хранилище ключей** из предложенных. Будет загружена страница создания хранилища ключей.
1. На странице создания хранилища ключей нажмите **Создать**.  
1. Заполните сведения для создания хранилища ключей и щелкните **Проверка + создание**, затем **Создать**.  
1. Перейдите к только что созданному хранилищу ключей, выбрав **Перейти к ресурсу** в уведомлении.  
1. Скопируйте **DNS-имя**. Это потребуется для следующего шага.  
1. Перейдите в **Секреты** и выберите **+ Создать/импортировать**.  
1. Введите название секрета и сохраните его для следующего этапа. В качестве значения используйте строку подключения, созданную на этапе для концентратора событий. Нажмите **Создать**.  
1. Щелкните **Политики доступа**, затем **+ Добавить политику доступа**.  
1. В разделе **Разрешения секретов** нажмите кнопку **Получить**, в разделе **Выбор субъекта** выберите **Отслеживание изменений в Microsoft Graph**. Щелкните **Добавить**.  

### <a name="creating-the-subscription-and-receiving-notifications"></a>Создание подписки и просмотр уведомлений

После создания обязательных служб хранилища Azure Key Vault и концентраторов событий Azure вы сможете создать свою подписку и начать получать уведомления об изменениях через концентраторы событий Azure.

#### <a name="creating-the-subcription"></a>Создание подписки

Подписки на изменение уведомлений с помощью концентраторов событий почти идентичны уведомлениям об изменениях с помощью веб-перехватчиков. Основное отличие заключается в том, что для доставки уведомлений используют концентраторы событий. Другие операции сходны, в том числе [создание подписки](/graph/api/subscription-post-subscriptions).  

Основное отличие в ходе создания подписки будет заключаться в значении **notificationUrl,**. Необходимо настроить его на `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>` со следующими значениями:

- `azurekeyvaultname` — название созданного хранилища ключей. Его можно найти в DNS-имени.
- `secretname` — название созданного секрета. Его можно найти на странице **Секреты** в хранилище Azure Key Vault.
- `domainname` — имя клиента, например, consto.onmicrosoft.com или contoso.com. Поскольку этот домен будет использоваться для доступа к хранилищу Azure Key Vault, важно, чтобы он соответствовал домену, используемому подпиской Azure с хранилищем Azure Key Vault. Чтобы получить эту информацию, вы можете перейти на страницу обзора созданного хранилища Azure Key Vault и щелкнуть на подписку. Имя домена выводится в поле **Каталог**.

#### <a name="receiving-notifications"></a>Получение уведомлений

События будут доставлены концентраторами событий в ваше приложение. Дополнительные сведения см. в статье [Получение событий](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) в документации по концентраторам событий.

Чтобы вы могли получать уведомления в приложении, потребуется создать еще одну политику общего доступа с разрешением на "Прослушивание" и получить строку подключения, как в инструкциях из раздела [Настройка концентратора событий Azure](#configuring-the-azure-event-hub).

> **Примечание**. Создайте отдельную политику для приложения, которое прослушивает сообщения в концентраторах событий, вместо того чтобы повторно использовать строку подключения, заданную в хранилище Azure KeyVault. Это гарантирует, что каждый компонент решения будет иметь только нужные разрешения в соответствии с принципом минимальных разрешений.

> **Примечание.** Ваше приложение будет получать сообщения о проверке каждый раз при создании новой подписки. Эти уведомления следует пропустить. В приведенном ниже примере представлен текст сообщения о проверке.

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

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a>Что произойдет, если приложение для отслеживания изменений в Microsoft Graph отсутствует?

Возможно, в вашем клиенте нет субъекта-службы **отслеживания изменений в Microsoft Graph**. Это зависит от того, когда был создан клиент и от административных операций. Чтобы устранить эту проблему, выполните [следующий запрос](https://developer.microsoft.com/en-us/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) в [проводнике Microsoft Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).

Сведения о запросе: `0bf30f3b-4a52-48df-9a82-234910c4a086` — глобальный идентификатор приложения для отслеживания изменений в Microsoft Graph.

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals

{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> **Примечание.** Вы можете получить отказ в выполнении этого запроса. В этом случае щелкните значок шестеренки рядом с именем своей учетной записи в левом верхнем углу. Затем выберите **Выбрать разрешения**, а затем выполните поиск по запросу **Application.ReadWrite.All**. Проверьте разрешения и выберите **Согласие**. После того как вы подтвердите новое разрешение, снова выполните поисковый запрос.

> **Примечание.** Этот API-интерфейс действует только для учебной или рабочей учетной записи, но не в личной учетной записи. Убедитесь, что вы вошли в систему через учетную запись в своем домене.

Кроме того, для добавления отсутствующего субъекта-службы можно использовать командлет PowerShell [New-MgServicePrincipal](/powershell/module/microsoft.graph.applications/new-mgserviceprincipal?view=graph-powershell-1.0&preserve-view=true) в Microsoft Graph. Ниже приведен пример сценария.

```PowerShell
Connect-Graph -Scopes "Application.ReadWrite.All"
New-MgServicePrincipal -AppId "0bf30f3b-4a52-48df-9a82-234910c4a086"
```

## <a name="next-steps"></a>Дальнейшие действия

См. следующие краткие руководства о концентраторах событий Azure:

- [.NET Core](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [Java](/azure/event-hubs/event-hubs-java-get-started-send)
- [Python](/azure/event-hubs/get-started-python-send-v2)
- [JavaScript](/azure/event-hubs/get-started-node-send-v2)
