---
title: Тип ресурса tenantRelationshipAccessPolicyBase
description: Базовый тип, который определяет отношение клиента.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d7fb506e09c88de18eb22153bc3608514ef19177
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604765"
---
# <a name="tenantrelationshipaccesspolicybase-resource-type"></a>Тип ресурса tenantRelationshipAccessPolicyBase

Пространство имен: microsoft.graph

Базовый тип, который определяет отношение клиента. Это абстрактный тип, наследуемый объектами межтенантной политики, включая [crossTenantAccessPolicy](crosstenantaccesspolicy.md).

Наследуется [от policyBase](policybase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| определение (не рекомендуется) | Коллекция String | Необработанные определения JSON политики межтенантного доступа. **Устарело. Не используйте.** |
| description | Строка | Описание этой политики. Обязательный элемент. Наследуется [от policyBase](../resources/policybase.md). |
| displayName | Коллекция String | Отображаемое имя для этой политики. Обязательный элемент. Наследуется [от policyBase](../resources/policybase.md). |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
