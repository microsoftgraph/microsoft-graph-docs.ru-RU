---
title: тип ресурса applicationServicePrincipal
description: Сочетание приложения и службыPrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 35abee6b3028111ce4237828b58492a546ff5d4b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476453"
---
# <a name="applicationserviceprincipal-resource-type"></a>тип ресурса applicationServicePrincipal

Пространство имен: microsoft.graph

При добавлении экземпляра приложения из галереи приложений [](../resources/application.md) Azure AD в каталоге создаются объекты приложения и [servicePrincipal.](../resources/serviceprincipal.md) **ApplicationServicePrincipal представляет** собой консатацию объекта **приложения** и **servicePrincipal.**

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство         | Тип                                                 | Описание                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| application      | [application](../resources/application.md)           | Представляет приложение, зарегистрированное в Azure Active Directory. |
| servicePrincipal | [servicePrincipal](../resources/serviceprincipal.md) | Представляет экземпляр приложения в каталоге.        |

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
  "servicePrincipal": { "@odata.type": "microsoft.graph.servicePrincipal" },
  "application": { "@odata.type": "microsoft.graph.application" }
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
