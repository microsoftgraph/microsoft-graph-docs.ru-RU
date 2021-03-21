---
title: тип ресурса fido2KeyRestrictions
description: Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fd319b64d124fc2c80c7f851a2e062d3568c2d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964959"
---
# <a name="fido2keyrestrictions-resource-type"></a>тип ресурса fido2KeyRestrictions

Пространство имен: microsoft.graph

Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей [безопасности FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|aaGuids|Коллекция строк|Коллекция GUID-интерфейсов проверки подлинности. AADGUID определяет ключевые типы и производителей.|
|enforcementType|fido2RestrictionEnforcementType|Тип правоприменения. Возможные значения: `allow`, `block`.|
|isEnforced|Boolean|Определяет, включено ли правоприменительных ключевых элементов.|

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
