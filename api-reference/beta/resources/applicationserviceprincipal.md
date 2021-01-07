---
title: Тип ресурса applicationServicePrincipal
description: Сочетание приложения и servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77d1d9beeab406896bda53e88e9043be0a99e8fe
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777723"
---
# <a name="applicationserviceprincipal-resource-type"></a>Тип ресурса applicationServicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При добавлении экземпляра приложения из коллекции приложений Azure AD в каталоге создаются объекты [application](../resources/application.md) и [servicePrincipal.](../resources/serviceprincipal.md) **ApplicationServicePrincipal** представляет собой совмещение объекта **application** и **servicePrincipal.**

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


