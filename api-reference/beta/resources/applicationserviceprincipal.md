---
title: Тип ресурса АппликатионсервицепринЦипал
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147938"
---
# <a name="applicationserviceprincipal-resource-type"></a>Тип ресурса АппликатионсервицепринЦипал

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При добавлении экземпляра приложения из коллекции приложений Azure AD объекты [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) создаются в каталоге. **АппликатионсервицепринЦипал** представляет сцепление объекта **Application** и **servicePrincipal** .

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство | Тип        | Описание |
|:-------------|:------------|:------------|
|application|[application](../resources/application.md)|Представляет приложение, зарегистрированное в Azure Active Directory.|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|Представляет экземпляр приложения в каталоге.|

## <a name="relationships"></a>Отношения

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
