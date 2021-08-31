---
title: тип ресурса unmanagedDevice
description: Неугомонное устройство, обнаруженное в сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0286d1ac8790cff207ff754d49cd6d3ee51986de
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806595"
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
|domain|Строка|Домен.|
|manufacturer|String|Производитель.|
|model|String|Модель.|
|location|Строка|Расположение.|
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



