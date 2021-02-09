---
title: Тип ресурса cloudPcOnPremisesConnection
description: Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для подключения к локальной сети для облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ec7a3dfaee2f1e111b81bc551f427764fce50f1b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159614"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>Тип ресурса cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для подключения к локальной сети для облачных компьютеров.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Get cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Чтение свойств и связей объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Обновление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Удаление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md) Нельзя удалить используемую связь.|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновление пароля домена AD для успешного [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор локального подключения. Только для чтения.|
|displayName|String|Отображаемого имени для локального подключения.|
|subscriptionId|String|ИД целевой подписки Azure, связанной с клиентом.|
|subscriptionName|String|Имя целевой подписки Azure. Только для чтения.|
|adDomainName|String|Полное доменное имя домена Active Directory, к нему нужно присоединиться.|
|adDomainUsername|String|Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), которая имеет разрешения на создание объектов-компьютеров в Active Directory. Необходимый формат: admin@contoso.com.|
|adDomainPassword|String|Пароль, связанный с adDomainUsername.|
|organizationalUnit|String|Подразделение, в котором создается учетная запись компьютера. Если оставить значение null, используется OU, настроенное в качестве используемого по умолчанию (известного контейнера объектов компьютера) в домене Active Directory (OU). Необязательный параметр.|
|resourceGroupId|String|ИД целевой группы ресурсов. Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|String|ИД целевой виртуальной сети. Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|String|ИД целевой подсети. Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки состояния, которая была сделана для локального подключения. Например, если состояние "passed", локальное подключение прошло все проверки, запускаемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверках состояния подключения и соответствующих результатах. Возвращается только в `$select` . Пример получения свойства **inUse** см. в примере 2. Получите выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|
|inUse|Boolean|Когда `true` используется локальное подключение. Когда `false` подключение не используется. Невозможно удалить используемую связь. Возвращается только с помощью оператора `$select`. Пример получения свойства **inUse** см. в примере 2. Получите выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>Значения cloudPcOnPremisesConnectionStatus

|Member|Описание|
|:---|:---|
|pending|Создано и ожидает проверки состояния.
|running|Запущены проверки состояния.|
|passed|Пройдены проверки состояния.|
|failed|Сбой проверки состояния.|
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
