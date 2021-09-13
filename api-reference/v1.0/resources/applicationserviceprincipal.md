---
title: тип ресурса applicationServicePrincipal
description: Сочетание приложения и службыPrincipal.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 3c5bafde4452842494f7890b8492b29e42bc8730
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078996"
---
# <a name="applicationserviceprincipal-resource-type"></a>тип ресурса applicationServicePrincipal

Пространство имен: microsoft.graph

При добавлении экземпляра приложения из галереи приложений [](../resources/application.md) Azure AD в каталоге создаются объекты приложения и [servicePrincipal.](../resources/serviceprincipal.md) **ApplicationServicePrincipal представляет** собой консатацию объекта **приложения** и **servicePrincipal.**

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство         | Тип                                                 | Описание                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| application      | [application](../resources/application.md)           | Представляет приложение, зарегистрированные в Azure Active Directory. |
| servicePrincipal | [servicePrincipal](../resources/serviceprincipal.md) | Представляет экземпляр приложения в каталоге.        |

## <a name="relationships"></a>Отношения

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
