---
title: hasPayloadLinkResultItem type
description: Класс, содержащий результат действия HasPayloadLinks.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 123177d4935ea7aec924345d27134f7ad779a625
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785691"
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



