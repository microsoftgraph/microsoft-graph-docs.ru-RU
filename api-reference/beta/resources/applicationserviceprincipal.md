---
title: Тип ресурса АппликатионсервицепринЦипал
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b45da6cd8533d9522d42428f6e222a669f17e681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050271"
---
# <a name="applicationserviceprincipal-resource-type"></a>Тип ресурса АппликатионсервицепринЦипал

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При добавлении экземпляра приложения из коллекции приложений Azure AD объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) создаются в каталоге. **АппликатионсервицепринЦипал** представляет сцепление объекта **Application** и **servicePrincipal** .

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство | Тип        | Описание |
|:-------------|:------------|:------------|
|application|[application](../resources/application.md)|Представляет приложение, зарегистрированное в Azure Active Directory.|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|Представляет экземпляр приложения в каталоге.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


