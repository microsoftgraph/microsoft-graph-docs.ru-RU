---
title: Тип ресурса Акцесспаккажересаурцеролескопе
description: Область применения роли пакета Access — это ссылка на область в ресурсе и роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ee4ec63c9c2efb60850ee7915e62dc0e284f8ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870964"
---
# <a name="accesspackageresourcerolescope-resource-type"></a>Тип ресурса Акцесспаккажересаурцеролескопе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)областью применения роли ресурса Package является ссылка на область в ресурсе и роль в этом ресурсе для этой области.  Пакет Access будет иметь доступ к областям роли ресурса пакета для ресурсов в каталоге, которые относятся к этому пакету Access.  Когда тема получает назначение пакета Access, тема будет подготовлена к работе с ролью в этой области каждой области применения роли ресурса пакета Access.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) | Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) | Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access. |
| [Создание Акцесспаккажересаурцеролескопе](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|String|Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|модифиедби|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажересаурцероле|[акцесспаккажересаурцероле](accesspackageresourcerole.md)| Только для чтения. Допускается значение null.|
|акцесспаккажересаурцескопе|[акцесспаккажересаурцескопе](accesspackageresourcescope.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
  }

}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
