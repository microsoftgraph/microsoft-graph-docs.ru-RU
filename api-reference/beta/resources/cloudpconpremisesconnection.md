---
title: Тип ресурса cloudPcOnPremisesConnection
description: Представляет определенную коллекцию сведений о ресурсах Azure, которые можно использовать для установки сетевого подключения Azure для облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3c6e3630ffe7ed1853c758ce14a32178ea835549
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733229"
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
|[RunHealthChecks объекта cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Выполните проверки работоспособности [для cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновите пароль домена Active Directory для [успешного подключения cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Этот API поддерживается, если тип объекта **cloudPcOnPremisesConnection** имеет значение `hybridAzureADJoin`.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сетевого подключения Azure. Только для чтения.|
|Managedby|[cloudPcManagementService](#cloudpcmanagementservice-values)|Указывает, какие службы управляют сетевым подключением Azure. Возможные значения: `windows365`и `devBox` `unknownFutureValue`. Только для чтения.
|type|[CloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|Указывает, как подготовленный облачный компьютер будет присоединен к Azure Active Directory. Значение по умолчанию — `hybridAzureADJoin`. Возможные значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|displayName|String|Отображаемое имя сетевого подключения Azure.|
|subscriptionId|String|Идентификатор целевой подписки Azure, связанной с клиентом.|
|subscriptionName|String|Имя целевой подписки Azure. Только для чтения.|
|adDomainName|String|Полное доменное имя (FQDN) домена Active Directory, к которому вы хотите присоединиться. Необязательный параметр.|
|adDomainUsername|String|Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), которая имеет разрешения на создание объектов-компьютеров в Active Directory. Обязательный формат: admin@contoso.com. Необязательный параметр.|
|adDomainPassword|String|Пароль, связанный с **adDomainUsername**.|
|organizationalUnit|String|Подразделение, в котором создается учетная запись компьютера. Если оставить значение NULL, используется подразделение, настроенное в качестве стандартного (хорошо известного контейнера объектов компьютера) в домене Active Directory. Необязательный параметр.|
|resourceGroupId|String|Идентификатор целевой группы ресурсов. Обязательный формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|String|Идентификатор целевой виртуальной сети. Обязательный формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|String|Идентификатор целевой подсети. Обязательный формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки работоспособности, выполненной в сетевом подключении Azure. Например, если состояние "передано", сетевое подключение Azure прошел все проверки, выполняемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверке работоспособности подключения и соответствующих результатах. Возвращается только в . `$select` Пример, показывающий, как получить свойство **inUse** , см. в примере 2. Получение выбранных свойств сетевого подключения [Azure, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|
|inUse|Boolean|Когда `true`используется сетевое подключение Azure. Если `false`подключение не используется. Невозможно удалить используемую связь. Возвращается только с помощью оператора `$select`. Пример, показывающий, как получить свойство **inUse** , см. в примере 2. Получение выбранных свойств сетевого подключения [Azure, включая healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Только для чтения.|

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
|unknownFutureValue|Неизвестное будущее состояние (зарезервировано, не используется сейчас).|

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
