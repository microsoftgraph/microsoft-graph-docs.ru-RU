---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6ef0827736d16f1dbf3aedfb664467011e75e7b2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383779"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>Тип ресурса Акцесспаккажеассигнментресаурцероле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Акцесспаккажеассигнментресаурцероле](../api/accesspackageassignmentresourcerole-get.md) | [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)  | Получение объекта Акцесспаккажеассигнментресаурцероле. |
| [Список Акцесспаккажеассигнментресаурцеролес](../api/accesspackageassignmentresourcerole-list.md) | Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md) | Получение списка объектов Акцесспаккажеассигнментресаурцероле. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|оригинид|String|Уникальный идентификатор, связанный с исходной системой. |
|оригинсистем|String|Система, в которой необходимо создать назначение роли или она была создана для назначения пакета Access, например `SharePointOnline` .|
|status|String|Значение задается, `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажеассигнментс|Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)| Назначения для пакетов Access, которые применяют это назначение роли. Только для чтения. Допускается значение null.|
|акцесспаккажересаурцероле|[акцесспаккажересаурцероле](accesspackageresourcerole.md)| Только для чтения. Допускается значение null.|
|акцесспаккажересаурцескопе|[акцесспаккажересаурцескопе](accesspackageresourcescope.md)| Только для чтения. Допускается значение null.|
|акцесспаккажесубжект|[акцесспаккажесубжект](accesspackagesubject.md)| Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
