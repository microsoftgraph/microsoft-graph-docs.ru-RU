---
title: тип ресурса cloudPcOnPremisesConnection
description: Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e56a960bc1dc8c7bc767cc7673c68ebee2c8ed4e
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672653"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>тип ресурса cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Get cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание нового [объекта cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Обновление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Удаление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление [объекта cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) . Вы не можете удалить используемую связь.|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [здоровья в cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновление пароля домена Active Directory для успешного [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Этот API поддерживается при типе **onPremisesConnection** `hybridAzureADJoin`.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор локального подключения. Только для чтения.|
|managedBy|[cloudPcManagementService](#cloudpcmanagementservice-values)|Указывает, какие службы управляют локальной связью. Возможные значения: `windows365`и `devBox` `unknownFutureValue`. Только для чтения.
|type|[cloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|Указывает, как будет присоединяться к Azure Active Directory. Значение по умолчанию — `hybridAzureADJoin`. Возможные значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|displayName|Строка|Имя отображения локального подключения.|
|subscriptionId|Строка|ID целевой подписки Azure, связанной с клиентом.|
|subscriptionName|Строка|Имя целевой подписки Azure. Только для чтения.|
|adDomainName|Строка|Полное доменное имя домена (FQDN) домена Active Directory, к нему необходимо присоединиться. Необязательное свойство.|
|adDomainUsername|String|Имя пользователя учетной записи Active Directory (учетная запись пользователя или службы), которая имеет разрешения на создание компьютерных объектов в Active Directory. Необходимый формат: admin@contoso.com. Необязательное свойство.|
|adDomainPassword|String|Пароль, связанный с **adDomainUsername**.|
|organizationalUnit|String|Организационное подразделение (OU), в котором создается учетная запись компьютера. Если оставить null, используется OU, настроенный как по умолчанию (хорошо известный контейнер объектов компьютера) в домене Active Directory (OU). Необязательное свойство.|
|resourceGroupId|Строка|ID целевой группы ресурсов. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Строка|ID целевой виртуальной сети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|Строка|ID целевой подсети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки состояния здоровья, которая проводится на локальном подключении. Например, если состояние "пройдено", локальное подключение прошло все проверки, запускаемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверках состояния подключения и соответствующих результатах. Возвращается только на `$select`. Пример получения свойства **inUse** см. в примере 2. Получить выбранные свойства локального подключения [, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|
|inUse|Boolean|Когда `true`используется локальное подключение. Когда `false`подключение не используется. Невозможно удалить используемую связь. Возвращается только на `$select`. Пример получения свойства **inUse** см. в примере 2. Получить выбранные свойства локального подключения [, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|

### <a name="cloudpcmanagementservice-values"></a>значения cloudPcManagementService

|Элемент| Значение |Описание|
|:---|:---|:---|
|windows365|1| Локальное подключение было успешно создано через Windows365.|
|devBox|2| Локальное подключение было успешно создано через Project Fidalgo.|
|unknownFutureValue|4| Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="cloudpconpremisesconnectiontype-values"></a>значения cloudPcOnPremisesConnectionType

|Member|Описание|
|:---|:---|
|hybridAzureADJoin|Присоединились к локальной службе Active Directory и Azure AD. Только гибридные пользователи могут быть назначены и войти в облачный компьютер.|
|azureADJoin|Присоединилась только к Azure AD. Пользователи только для облачных и гибридных сетей могут быть назначены и войти в облачный компьютер.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>значения cloudPcOnPremisesConnectionStatus

|Member|Описание|
|:---|:---|
|ожидание|Создано и ожидается проверка состояния здоровья.|
|запуск|Проверка состояния здоровья запущена.|
|прошло|Проверка состояния здоровья прошла.|
|не удалось|Проверка состояния не удалась.|
|warning|Проверки состояния здоровья прошли с предупреждением.|
|unknownFutureValue|Неизвестный будущий статус (зарезервирован, не используется прямо сейчас).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false,
  "optionalProperties": ["healthCheckStatusDetails"]
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "String (identifier)",
  "managedBy": "String",
  "type": "String",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "adDomainName": "String",
  "adDomainUsername": "String",
  "adDomainPassword": "String",
  "organizationalUnit": "String",
  "resourceGroupId": "String",
  "virtualNetworkId": "String",
  "subnetId": "String",
  "healthCheckStatus": "string",
  "healthCheckStatusDetails": {
    "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "healthChecks": [
      {
        "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
        "displayName": "String",
        "status": "String",
        "startDateTime": "String (timestamp)",
        "endDateTime": "String (timestamp)",
        "errorType": "String",
        "recommendedAction": "String",
        "additionalDetails": "String"
      }
    ]
  },
  "inUse": "Boolean"
}
```
