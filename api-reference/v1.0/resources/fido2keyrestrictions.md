---
title: тип ресурса fido2KeyRestrictions
description: Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37b9e2c7a66b3ce9a43c08560f5e5f4a8e0acc2e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036531"
---
# <a name="fido2keyrestrictions-resource-type"></a>тип ресурса fido2KeyRestrictions

Пространство имен: microsoft.graph

Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей [безопасности FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|aaGuids|Коллекция String|Коллекция GUID Authenticator проверки. AADGUID определяет ключевые типы и производителей.|
|enforcementType|fido2RestrictionEnforcementType|Тип правоприменения. Возможные значения: `allow`, `block`.|
|isEnforced|Логический|Определяет, включено ли правоприменительных ключевых элементов.|

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
