---
title: тип ресурса fido2KeyRestrictions
description: Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 29ec1327da2104ba14fcfb73cd4374453417f8c2c2f5cb1b10012131918f9baa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149942"
---
# <a name="fido2keyrestrictions-resource-type"></a>тип ресурса fido2KeyRestrictions

Пространство имен: microsoft.graph

Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей [безопасности FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|aaGuids|Коллекция String|Коллекция GUID Authenticator проверки. AADGUID определяет ключевые типы и производителей.|
|enforcementType|fido2RestrictionEnforcementType|Тип правоприменения. Возможные значения: `allow`, `block`.|
|isEnforced|Логическое|Определяет, включено ли правоприменительных ключевых элементов.|

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
