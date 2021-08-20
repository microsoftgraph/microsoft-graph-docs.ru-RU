---
title: hasPayloadLinkResultItem type
description: Класс, содержащий результат действия HasPayloadLinks.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f96999c5a144a736a0ac8070d725245b59e8ed1c9c67e2c1301fded9cc7742a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235963"
---
# <a name="haspayloadlinkresultitem-resource-type"></a>hasPayloadLinkResultItem type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий результат действия HasPayloadLinks.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|payloadId|Строка|Ключ полезной нагрузки в формате Guid.|
|hasLink|Логический|Указать, есть ли у полезной нагрузки ссылки или нет.|
|error|Строка|Сведения об исключении указывают, была ли проверка этого элемента успешной или нет. Пустая строка без ошибок.|
|sources|[коллекция deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Причина, по которой происходит ссылка.|

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




