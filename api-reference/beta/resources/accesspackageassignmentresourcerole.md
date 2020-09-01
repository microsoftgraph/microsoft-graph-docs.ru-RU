---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 403b97dc335e57dfd2d4f2fe2aa75c4f6fd07682
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319521"
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
|оригинид|String|Уникальный идентификатор, относящийся к исходной системе, соответствующий свойству Оригинид объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md). |
|оригинсистем|String|Система, в которой необходимо создать назначение роли или она была создана для назначения пакета Access, например `SharePointOnline` , `AadGroup` или `AadApplication` соответствующего свойству оригинсистем объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md).|
|status|String|Это значение используется, `PendingFulfillment` когда назначение пакета Access еще не было доставлено в исходную систему, и `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.|

## <a name="relationships"></a>Отношения

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
