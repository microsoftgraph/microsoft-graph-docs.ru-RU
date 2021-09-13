---
title: тип ресурса unmanagedDevice
description: Неугомонное устройство, обнаруженное в сети.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1606ba0aaedc46ea9a27f6d7d8a0565480c59a01
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100976"
---
# <a name="unmanageddevice-resource-type"></a>тип ресурса unmanagedDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Неугомонное устройство, обнаруженное в сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|os|String|Операционная система.|
|osVersion|String|Версия операционной системы.|
|ipAddress|String|IP-адрес.|
|deviceName|String|Имя устройства.|
|macAddress|String|MAC-адрес.|
|domain|String|Домен.|
|manufacturer|String|Производитель.|
|model|String|Модель.|
|location|String|Расположение.|
|lastLoggedOnUser|String|Последний вход на пользователя.|
|lastSeenDateTime|DateTimeOffset|Последний раз видели дату и время.|

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



