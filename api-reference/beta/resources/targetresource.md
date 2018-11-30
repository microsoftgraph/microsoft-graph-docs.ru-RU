---
title: Тип ресурса targetResource
description: Указывает коллекцию конечных типов ресурсов, связанные с действием аудита. Каждый тип целевого ресурса наследуют свойства, используйте следующий из данного ресурса.
ms.openlocfilehash: ba3bee7ce89f73ed97610d62676c22d14488ed9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075229"
---
# <a name="targetresource-resource-type"></a>Тип ресурса targetResource
Указывает коллекцию конечных типов ресурсов, связанные с действием аудита. Каждый тип целевого ресурса наследуют свойства, используйте следующий из данного ресурса.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает отображаемое имя, описанные в разделе типы назначения ресурсов ниже ресурсов.|
|id|String|Указывает уникальный идентификатор ресурса (например: идентификатор пользователя, AppId, RoleId.).|
|modifiedProperties|[modifiedProperty](modifiedproperty.md) коллекции|Указывает имя, старое значение и новое значение каждого атрибута, которые изменены. Этот параметр доступен для всех действий, «Обновить»|

### <a name="target-resource-types"></a>Типы назначения ресурсов

Тип ресурса конечного зависит от базового ресурса:

|Имя ресурса| Справочные материалы|
|-------------|----------|
Устройство|[targetResourceDevice](targetresourcedevice.md)
Каталог|[targetResourceDirectory] (targetresourcedirectory.md]
Group|[targetResourceGroup](targetresourcegroup.md)
Политика|[targetResourcePolicy](targetresourcepolicy.md)
Role|[targetResourceRole](targetresourcerole.md)
Участников-служб|[targetResourceServicePrincipal](targetresourceserviceprincipal.md)
User|[targetResourceUser](targetresourceuser.md)
Other (другие)|[targetResourceOther](targetresourceother.md)

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->