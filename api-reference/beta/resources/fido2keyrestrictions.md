---
title: Тип ресурса fido2KeyRestrictions
description: Представляет ключевые ограничения, которые применяются в рамках политики методов проверки подлинности для ключа безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c606b1d7bdbf604bd5109379bffb2c1a20f60730
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418422"
---
# <a name="fido2keyrestrictions-resource-type"></a>Тип ресурса fido2KeyRestrictions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ключевые ограничения, которые применяются в рамках [политики методов проверки подлинности для ключа безопасности FIDO2](../resources/fido2authenticationmethodconfiguration.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|аагуидс|Коллекция String|Коллекция идентификаторов GUID аттестации проверки подлинности. Аадгуидс определение типов ключей и производителей.|
|енфорцементтипе|fido2RestrictionEnforcementType|Тип принудительного применения. Возможные значения: `allow`, `block`.|
|Принудительное применение|Boolean|Определяет, включено ли настроенное применение ключа.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
