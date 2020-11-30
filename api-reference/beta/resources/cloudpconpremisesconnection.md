---
title: Тип ресурса Клаудпконпремисесконнектион
description: Представляет определенную коллекцию сведений о ресурсе Azure, которую можно использовать для установления подключения к локальной сети для облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a8ac0dea68aaac8c1f720948041cfd1eddc048f6
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378524"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>Тип ресурса Клаудпконпремисесконнектион

Пространство имен: microsoft.graph

Представляет определенную коллекцию сведений о ресурсе Azure, которую можно использовать для установления подключения к локальной сети для облачных компьютеров.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Онпремисесконнектионс](../api/virtualendpoint-list-onpremisesconnections.md)|Коллекция [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Получение Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-get.md)|[клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Чтение свойств и связей объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Создание Клаудпконпремисесконнектион](../api/virtualendpoint-post-onpremisesconnections.md)|[клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Создание нового объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Обновление Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-update.md)|[клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Обновление свойств объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Удаление Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-delete.md)|Нет|Удаление объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) . Вы не можете удалить используемое подключение.|
|[Рунхеалсчеккс из Клаудпконпремисесконнектион](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Выполните проверки работоспособности в [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для локального подключения. Только для чтения.|
|displayName|Строка|Отображаемое имя для локального подключения.|
|subscriptionId|Строка|Идентификатор целевой подписки Azure, связанной с клиентом.|
|субскриптионнаме|Строка|Имя целевой подписки Azure. Только для чтения.|
|аддомаиннаме|Строка|Полное доменное имя (FQDN) домена Active Directory, к которому нужно присоединиться.|
|аддомаинусернаме|Строка|Имя пользователя учетной записи Active Directory (учетной записи пользователя или службы), имеющей разрешения на создание объектов компьютеров в Active Directory. Требуемый формат: contoso@microsoft.com.|
|аддомаинпассворд|Строка|Пароль, связанный с Аддомаинусернаме.|
|organizationalUnit|Строка|Подразделение (OU), в котором создается учетная запись компьютера. Если оставить значение null, то используется подразделение, настроенное по умолчанию (хорошо известный контейнер объектного компьютера) в домене Active Directory (OU). Необязательный параметр.|
|ресаурцеграупид|Строка|Идентификатор целевой группы ресурсов. Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}".|
|виртуалнетворкид|Строка|Идентификатор целевой виртуальной сети. Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкнаме}".|
|субнетид|Строка|Идентификатор целевой подсети. Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.Нетворк/виртуалнетворкс/{виртуалнетворкид}/субнетс/{субнетнаме}".|
|хеалсчеккстатус|клаудпконпремисесконнектионстатус|Состояние последней проверки работоспособности, выполненной для локального подключения. Например, если задано состояние "передано", для локального подключения пройдет все проверки, запущенные службой. Только для чтения. Возможные значения: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|хеалсчеккстатусдетаилс|[клаудпконпремисесконнектионстатусдетаилс](../resources/cloudpconpremisesconnectionstatusdetails.md)|Сведения о проверках работоспособности подключения и соответствующие результаты. Возвращается только с помощью оператора `$select`. В этом [примере](../api/cloudpconpremisesconnection-get.md) показано, как получить свойство хеалсчеккстатусдетаилс. Только для чтения.|
|Используемых|Boolean|Если задано значение true, локальное подключение используется. Если значение равно false, соединение не используется. Невозможно удалить используемое подключение. Только для чтения.|

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
