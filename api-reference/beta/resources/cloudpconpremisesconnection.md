---
title: Тип ресурса cloudPcOnPremisesConnection
description: Представляет определенную коллекцию сведений о ресурсах Azure, которые можно использовать для установки сетевого подключения Azure для облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 10088c87531c250b24314f5df4b9bae3a842e31a
ms.sourcegitcommit: da9079132db3261aed80e6fc4b9314d16e0847b3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2022
ms.locfileid: "66186948"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>Тип ресурса cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенную коллекцию сведений о ресурсах Azure, которые можно использовать для установки сетевого подключения Azure для облачных компьютеров.

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Получение cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Чтение свойств и связей объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создайте объект [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Обновление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Удаление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) . Невозможно удалить используемую связь.|
|[RunHealthChecks объекта cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Отсутствует|Выполните проверки работоспособности [для cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновите пароль домена Active Directory для [успешного подключения cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Этот API поддерживается, если тип объекта **cloudPcOnPremisesConnection** имеет значение `hybridAzureADJoin`.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|adDomainName|String|Полное доменное имя (FQDN) домена Active Directory, к которому вы хотите присоединиться. Необязательное свойство.|
|adDomainPassword|String|Пароль, связанный с **adDomainUsername**.|
|adDomainUsername|String|Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), которая имеет разрешения на создание объектов-компьютеров в Active Directory. Обязательный формат: `admin@contoso.com`. Необязательное свойство.|
|alternateResourceUrl|String|URL-адрес интерфейса ресурса службы партнеров, который связывается с этим сетевым подключением Azure. Возвращается только на `$select`.|
|displayName|String|Отображаемое имя сетевого подключения Azure.|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки работоспособности, выполненной в сетевом подключении Azure. Например, если состояние равно `passed`, сетевое подключение Azure прошел все проверки, выполняемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверке работоспособности подключения и соответствующих результатах. Возвращается только на `$select`. Пример, показывающий, как получить свойство **inUse** , см. в примере 2. Получение выбранных свойств сетевого подключения [Azure, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|
|id|String|Уникальный идентификатор сетевого подключения Azure. Только для чтения.|
|inUse|Boolean|Когда `true`используется сетевое подключение Azure. Если `false`подключение не используется. Невозможно удалить используемую связь. Возвращается только на `$select`. Пример, показывающий, как получить свойство **inUse** , см. в примере 2. Получение выбранных свойств сетевого подключения [Azure, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|
|Managedby|[cloudPcManagementService](#cloudpcmanagementservice-values)|Указывает, какие службы управляют сетевым подключением Azure. Возможные значения: `windows365`, `devBox,` `unknownFutureValue`. Только для чтения.|
|organizationalUnit|String|Подразделение, в котором создается учетная запись компьютера. Если оставить значение NULL, используется подразделение, настроенное в качестве стандартного (хорошо известного контейнера объектов компьютера) в домене Active Directory. Необязательное свойство.|
|resourceGroupId|String|Идентификатор целевой группы ресурсов. Обязательный формат: `/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}`.|
|subnetId|String|Идентификатор целевой подсети. Обязательный формат: `/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}`.|
|subscriptionId|String|Идентификатор целевой подписки Azure, связанной с клиентом.|
|subscriptionName|String|Имя целевой подписки Azure. Только для чтения.|
|type|[CloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|Указывает, как подготовленный облачный компьютер будет присоединен к Azure Active Directory. Значение по умолчанию — `hybridAzureADJoin`. Возможные значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|virtualNetworkId|String|Идентификатор целевой виртуальной сети. Обязательный формат: `/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}`.|

### <a name="cloudpcmanagementservice-values"></a>Значения cloudPcManagementService

|Элемент| Значение |Описание|
|:---|:---|:---|
|windows365|1| Сетевое подключение Azure было успешно создано через Windows 365.|
|devBox|2| Сетевое подключение Azure успешно создано с помощью Project Fidalgo.|
|unknownFutureValue|4| Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="cloudpconpremisesconnectiontype-values"></a>Значения cloudPcOnPremisesConnectionType

|Member|Описание|
|:---|:---|
|hybridAzureADJoin|Присоединено к локальная служба Active Directory и Azure AD. На облачный компьютер могут быть назначены только гибридные пользователи.|
|azureADJoin|Присоединено только к Azure AD. Облачных и гибридных пользователей можно назначить и войти на облачный компьютер.|
|unknownFutureValue|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>Значения cloudPcOnPremisesConnectionStatus

|Member|Описание|
|:---|:---|
|Ожидающие|Создано и ожидается проверка работоспособности.|
|Запущена|Выполняются проверки работоспособности.|
|Прошло|Пройдены проверки работоспособности.|
|Сбой при|Сбой проверок работоспособности.|
|warning|Проверки работоспособности пройдены с предупреждением.|
|unknownFutureValue|Значение sentinel для развиваемого перечисления. Не следует использовать.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
  "adDomainName": "String",
  "adDomainPassword": "String",
  "adDomainUsername": "String",
  "alternateResourceUrl": "String",
  "displayName": "String",
  "healthCheckStatus": "String",
  "healthCheckStatusDetails": {
    "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
    "endDateTime": "String (timestamp)",
    "healthChecks": [
      { 
        "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
        "additionalDetails": "String",
        "displayName": "String",
        "endDateTime": "String (timestamp)",
        "errorType": "String",
        "recommendedAction": "String",
        "startDateTime": "String (timestamp)",
        "status": "String"
      }
    ],
    "startDateTime": "String (timestamp)"
  },
  "id": "String (identifier)",
  "inUse": "Boolean",
  "managedBy": "String",
  "organizationalUnit": "String",
  "resourceGroupId": "String",
  "subnetId": "String",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "type": "String",
  "virtualNetworkId": "String"
}
```
