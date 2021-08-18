---
title: тип ресурса cloudPcOnPremisesConnection
description: Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 57c8ca98935a11d053f91b9a971db2a0c436be65
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260655"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>тип ресурса cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Get cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание нового [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Обновление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Удаление cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md) Вы не можете удалить используемую связь.|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [здоровья в cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Нет|Обновление пароля домена AD для успешного [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор локального подключения. Только для чтения.|
|displayName|Строка|Имя отображения локального подключения.|
|subscriptionId|Строка|ID целевой подписки Azure, связанной с клиентом.|
|subscriptionName|Строка|Имя целевой подписки Azure. Только для чтения.|
|adDomainName|Строка|Полное доменное имя домена (FQDN) домена Active Directory, к нему необходимо присоединиться.|
|adDomainUsername|Строка|Имя пользователя учетной записи Active Directory (учетная запись пользователя или службы), которая имеет разрешения на создание компьютерных объектов в Active Directory. Необходимый формат: admin@contoso.com.|
|adDomainPassword|String|Пароль, связанный с **adDomainUsername**.|
|organizationalUnit|Строка|Организационное подразделение (OU), в котором создается учетная запись компьютера. Если оставить null, используется OU, настроенный как по умолчанию (хорошо известный контейнер объектов компьютера) в домене Active Directory (OU). Необязательное свойство.|
|resourceGroupId|Строка|ID целевой группы ресурсов. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|String|ID целевой виртуальной сети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|String|ID целевой подсети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|Состояние последней проверки состояния здоровья, которая проводится на локальном подключении. Например, если состояние "пройдено", локальное подключение прошло все проверки, запускаемые службой. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверках состояния подключения и соответствующих результатах. Возвращается только `$select` на . Пример, который показывает, как получить свойство **inUse,** см. в примере 2. Получить выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|
|inUse|Логический|Когда `true` используется локальное подключение. Когда `false` подключение не используется. Невозможно удалить используемую связь. Возвращается только с помощью оператора `$select`. Пример, который показывает, как получить свойство **inUse,** см. в примере 2. Получить выбранные свойства локального подключения, включая [healthCheckStatusDetails.](../api/cloudpconpremisesconnection-get.md) Только для чтения.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>значения cloudPcOnPremisesConnectionStatus

|Member|Описание|
|:---|:---|
|ожидание|Создано и ожидается проверка состояния здоровья.
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
