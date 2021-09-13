---
title: тип ресурса deviceLogCollectionResponse
description: Windows Объект запроса коллекции журналов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5727156187200a35d3d1d1ddfc8c30fb942f620e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091344"
---
# <a name="devicelogcollectionresponse-resource-type"></a>тип ресурса deviceLogCollectionResponse

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Объект запроса коллекции журналов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceLogCollectionResponses](../api/intune-devices-devicelogcollectionresponse-list.md)|[коллекция deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Список свойств и связей [объектов deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Get deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Чтение свойств и связей [объекта deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Создание deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Создайте новый [объект deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Удаление deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-delete.md)|Нет|Удаляет [устройствоLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).|
|[Обновление deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Обновление свойств объекта [deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Действие createDownloadUrl](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор в виде tenantId_deviceId_requestId|
|status|String|Состояние запроса на коллекцию журналов|
|managedDeviceId|Guid|Id устройства|
|errorCode|Int64|Код ошибки, если таковое есть. Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18|
|requestedDateTimeUTC|DateTimeOffset|DateTime запроса|
|receivedDateTimeUTC|DateTimeOffset|DateTime, в который был получен запрос|
|initiatedByUserPrincipalName|String|UpN для тех, кто инициировал запрос|
|expirationDateTimeUTC|DateTimeOffset|DateTime истечения срока действия журналов|
|size|Двойное с плавающей точкой|Размер журналов. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

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



