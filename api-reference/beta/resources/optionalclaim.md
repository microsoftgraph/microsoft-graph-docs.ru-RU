---
title: Тип ресурса optionalClaim
description: Содержит необязательное утверждение, связанное с приложением.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5e21ab86fb3ef34edea546546211782906e04251
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128542"
---
# <a name="optionalclaim-resource-type"></a>Тип ресурса optionalClaim

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит необязательное утверждение, связанное с [приложением](application.md) <!-- or a service principal -->. Свойства **idToken,** **accessToken** и **saml2Token** ресурса [optionalClaims](optionalclaims.md) — это коллекция **optionalClaim.** Если поддерживается определенным утверждением, можно также изменить поведение optionalClaim с помощью `additionalProperties` свойства. 

Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|additionalProperties|Коллекция объектов string| Дополнительные свойства утверждения. Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве name. |
|essential|Boolean| Если значение имеет значение true, утверждение, указанное клиентом, необходимо для обеспечения плавной авторизации для конкретной задачи, запрашиваемой конечным пользователем. Значение по умолчанию  false.|
|name|String| Имя необязательного утверждения. |
|source|Строка| Источник (объект каталога) утверждения. Существуют предварительно определенные утверждения и пользовательские утверждения из свойств расширения. Если значение источника — null, утверждение является предварительно заранее задаваемой необязательной заявкой. Если исходным значением является пользователь, значением в свойстве name является свойство расширения объекта user. |

## <a name="json-representation"></a>Представление в формате JSON

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
