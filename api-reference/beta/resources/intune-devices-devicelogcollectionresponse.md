---
title: Тип ресурса Девицелогколлектионреспонсе
description: Сущность запроса для сбора журналов Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a4316655cc7ca10205165bac1b96579eb135713
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060163"
---
# <a name="devicelogcollectionresponse-resource-type"></a>Тип ресурса Девицелогколлектионреспонсе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность запроса для сбора журналов Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицелогколлектионреспонсес](../api/intune-devices-devicelogcollectionresponse-list.md)|Коллекция [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md)|Список свойств и связей объектов [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Получение Девицелогколлектионреспонсе](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Чтение свойств и связей объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Создание Девицелогколлектионреспонсе](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Создание нового объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Удаление Девицелогколлектионреспонсе](../api/intune-devices-devicelogcollectionresponse-delete.md)|Нет|Удаляет объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md).|
|[Обновление Девицелогколлектионреспонсе](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Обновление свойств объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Действие createDownloadUrl](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор в виде tenantId_deviceId_requestId|
|status|String|Состояние запроса на сбор журналов|
|манажеддевицеид|Guid|Идентификатор устройства|
|errorCode|Int64|Код ошибки (при наличии). Допустимые значения — 9.22337203685478 E + 18 — 9.22337203685478 E + 18|
|рекуестеддатетимеутк|DateTimeOffset|Дата и время запроса|
|рецеиведдатетимеутк|DateTimeOffset|Дата и время получения запроса|
|Свойства initiatedbyuserprincipalname|String|Имя участника-пользователя, который инициировал запрос.|
|експиратиондатетимеутк|DateTimeOffset|Дата и время истечения срока действия журналов|
|size|Двойное с плавающей точкой|Размер журналов. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "managedDeviceId": "Guid",
  "errorCode": 1024,
  "requestedDateTimeUTC": "String (timestamp)",
  "receivedDateTimeUTC": "String (timestamp)",
  "initiatedByUserPrincipalName": "String",
  "expirationDateTimeUTC": "String (timestamp)",
  "size": "4.2"
}
```






