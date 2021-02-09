---
title: Тип ресурса unmanagedDevice
description: Неугодное устройство, обнаруженное в сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0163fb0f3704bee86622574428954b3c3c9f805a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160643"
---
# <a name="unmanageddevice-resource-type"></a>Тип ресурса unmanagedDevice

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Неугодное устройство, обнаруженное в сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|os|String|Операционная система.|
|osVersion|String|Версия операционной системы.|
|ipAddress|String|IP-адрес.|
|deviceName|String|Имя устройства.|
|macAddress|String|MAC-адрес.|
|domain|String|Домен.|
|manufacturer|String|Изготовитель.|
|model|String|Модель.|
|расположение;|String|Расположение.|
|lastLoggedOnUser|String|Последний вход пользователя.|
|lastSeenDateTime|DateTimeOffset|Дата и время последнего просмотров.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```




