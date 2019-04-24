---
title: Тип ресурса Модифиедпроперти
description: Указывает все измененные свойства со старым значением и новым значением для всех ресурсов в Azure AD, которые были изменены
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506238"
---
# <a name="modifiedproperty-resource-type"></a>Тип ресурса Модифиедпроперти
Указывает все измененные свойства со старым значением и новым значением для всех ресурсов в Azure AD, которые были изменены



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Указывает имя свойства целевого атрибута, которое было изменено.|
|newValue|String|Указывает обновленное значение для правильной работы.|
|oldValue|String|Указывает предыдущее значение свойства (перед обновлением).|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
