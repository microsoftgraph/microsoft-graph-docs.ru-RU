---
title: тип ресурса unmanagedDevice
description: Неугомонное устройство, обнаруженное в сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b98dee94642102bc067efd9b6d8c228d329b406a32ed7c6a8742099f0a60934a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206230"
---
# <a name="unmanageddevice-resource-type"></a>тип ресурса unmanagedDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Неугомонное устройство, обнаруженное в сети.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|os|Строка|Операционная система.|
|osVersion|String|Версия операционной системы.|
|ipAddress|String|IP-адрес.|
|deviceName|String|Имя устройства.|
|macAddress|Строка|MAC-адрес.|
|domain|String|Домен.|
|manufacturer|String|Производитель.|
|model|String|Модель.|
|location|String|Расположение.|
|lastLoggedOnUser|Строка|Последний вход на пользователя.|
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




