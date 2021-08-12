---
title: тип ресурса optionalClaim
description: ОПИСАНИЕ ЗДЕСЬ
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: a4302ac786dea126dad20562a8fbaa9aec3bd4128d3c4f4c315f30dc538b2661
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180595"
---
# <a name="optionalclaim-resource-type"></a>тип ресурса optionalClaim

Пространство имен: microsoft.graph

Содержит необязательный иск, связанный с [приложением](application.md) <!-- or a service principal -->. И `idToken` `accessToken` свойства ресурса `saml2Token` [optionalClaims](optionalclaims.md) — это коллекция **необязательныхClaim.** При поддержке определенного утверждения можно также изменить поведение необязательныйClaim с помощью `additionalProperties` свойства.

Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|additionalProperties|Коллекция String| Дополнительные свойства утверждения. Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве имени. |
|essential|Логическое| Если значение верно, утверждение, указанное клиентом, необходимо для обеспечения плавного доступа к авторизации для определенной задачи, запрашиваемой конечным пользователем. Значение по умолчанию  false.|
|name|String| Имя необязательного утверждения. |
|source|String| Источник (объект каталога) утверждения. Есть предопределяемые утверждения и пользовательские утверждения из свойств расширения. Если исходным значением является null, то утверждение является предопределяемой необязательной претензией. Если исходным значением является пользователь, значение в свойстве имени — это свойство расширения от объекта пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
