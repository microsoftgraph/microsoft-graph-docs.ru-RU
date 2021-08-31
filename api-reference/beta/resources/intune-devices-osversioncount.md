---
title: тип ресурса osVersionCount
description: Количество устройств с вредоносными программами для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5160cd66e6c18caa81c449e7cd9f661204bfdc87
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757953"
---
# <a name="osversioncount-resource-type"></a>тип ресурса osVersionCount

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств с вредоносными программами для каждой версии ОС

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|osVersion|String|Версия ОС|
|deviceCount|Int32|Количество устройств с вредоносными программами для версии ОС|
|lastUpdateDateTime|DateTimeOffset|Время последнего обновления для подсчета устройств в UTC|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```



