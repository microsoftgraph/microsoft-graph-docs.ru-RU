---
title: Тип ресурса fido2KeyRestrictions
description: Представляет ключевые ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a40a185f688038d3c849113ae8e9b53c4f0652f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133800"
---
# <a name="fido2keyrestrictions-resource-type"></a>Тип ресурса fido2KeyRestrictions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ключевые ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|aaGuids|Коллекция объектов string|Коллекция GUID аутентификации. AADGUID определяют ключевые типы и изготовителей.|
|enforcementType|fido2RestrictionEnforcementType|Тип принуителя. Возможные значения: `allow`, `block`.|
|isEnforced|Boolean|Определяет, включено ли настроено правопримение ключа.|

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
