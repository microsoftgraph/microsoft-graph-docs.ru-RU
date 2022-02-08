---
title: тип ресурса tenantRelationshipAccessPolicyBase
description: 'Базовый тип, определяя отношения клиента.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="tenantrelationshipaccesspolicybase-resource-type"></a>тип ресурса tenantRelationshipAccessPolicyBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый тип, определяя отношения клиента. Это абстрактный тип, унаследованный объектами политики меж клиента, включая [crossTenantAccessPolicy](crosstenantaccesspolicy.md).

Наследует [от policyBase](policybase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| определение (неподготовленное) | Коллекция объектов string | Необработанные определения JSON политики меж клиента доступа. **Устарело. Не используйте.** |
| description | Строка | Описание этой политики. Обязательный. Унаследовано от [policyBase](../resources/policybase.md). |
| displayName | Коллекция объектов string | Отображение имени для этой политики. Обязательный. Унаследовано от [policyBase](../resources/policybase.md). |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationshipAccessPolicyBase",
  "definition": [
    "String"
  ],
  "description": "String",
  "displayName": "String"
}
```
