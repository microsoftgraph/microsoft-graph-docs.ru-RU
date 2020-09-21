---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56c5631ed85f68942758b1283128f4f24ca53d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993506"
---
# <a name="haspayloadlinkresultitem-resource-type"></a>Тип ресурса Хаспайлоадлинкресултитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий результат действия Хаспайлоадлинкс.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|пайлоадид|String|Ключ полезных данных в формате GUID.|
|хаслинк|Boolean|Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.|
|error|String|Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.|
|sources|Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Причина, по которой получена ссылка.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```






