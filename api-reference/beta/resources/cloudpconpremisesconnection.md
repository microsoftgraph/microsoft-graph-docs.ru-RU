---
title: тип ресурса cloudPcOnPremisesConnection
description: Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: cb1b3dc86aa941720411db9f577e2b12a5817151
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266012"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>тип ресурса cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Get cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание нового [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Обновление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Удаление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md) Вы не можете удалить используемую связь.|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [здоровья в cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновление пароля домена Active Directory для успешного [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Этот API поддерживается при типе **onPremisesConnection** `hybridAzureADJoin` .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор локального подключения. Только для чтения.|
|type|[cloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|Указывает, как будет присоединяться к Azure Active Directory. Значение по умолчанию — `hybridAzureADJoin`. Возможные значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|displayName|Строка|Имя отображения локального подключения.|
|subscriptionId|Строка|ID целевой подписки Azure, связанной с клиентом.|
|subscriptionName|Строка|Имя целевой подписки Azure. Только для чтения.|
|adDomainName|Строка|Полное доменное имя домена (FQDN) домена Active Directory, к нему необходимо присоединиться. Необязательно.|
|adDomainUsername|Строка|Имя пользователя учетной записи Active Directory (учетная запись пользователя или службы), которая имеет разрешения на создание компьютерных объектов в Active Directory. Необходимый формат: admin@contoso.com. Необязательно.|
|adDomainPassword|Строка|Пароль, связанный с **adDomainUsername**.|
|organizationalUnit|Строка|Организационное подразделение (OU), в котором создается учетная запись компьютера. Если оставить null, используется OU, настроенный как по умолчанию (хорошо известный контейнер объектов компьютера) в домене Active Directory (OU). Необязательно.|
|resourceGroupId|Строка|ID целевой группы ресурсов. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Строка|ID целевой виртуальной сети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|Строка|ID целевой подсети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки состояния здоровья, которая проводится на локальном подключении. Например, если состояние "пройдено", локальное подключение прошло все проверки, запускаемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверках состояния подключения и соответствующих результатах. Возвращается только `$select` на . Пример, который показывает, как получить свойство **inUse,** см. в примере 2. Получить выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|
|inUse|Логическое|Когда `true` используется локальное подключение. Когда `false` подключение не используется. Невозможно удалить используемую связь. Возвращается только с помощью оператора `$select`. Пример, который показывает, как получить свойство **inUse,** см. в примере 2. Получить выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|

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
