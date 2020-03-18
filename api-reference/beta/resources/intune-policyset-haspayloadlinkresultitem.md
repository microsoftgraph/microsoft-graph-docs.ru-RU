---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 46568e386c2896db307f78cc12205c115605a76e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775908"
---
# <a name="haspayloadlinkresultitem-resource-type"></a>Тип ресурса Хаспайлоадлинкресултитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий результат действия Хаспайлоадлинкс.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|пайлоадид|String|Ключ полезных данных в формате GUID.|
|хаслинк|Логический|Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.|
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



