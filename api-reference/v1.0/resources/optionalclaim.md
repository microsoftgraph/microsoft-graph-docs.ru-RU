---
title: Тип ресурса Оптионалклаим
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 355a9e558f76a8dd38ea227950bb9c3938aa21c4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869817"
---
# <a name="optionalclaim-resource-type"></a>Тип ресурса Оптионалклаим

Содержит необязательное утверждение, связанное с [приложением](application.md) <!-- or a service principal -->. Свойства `idToken`, `accessToken`и `saml2Token` , в ресурсе [оптионалклаимс](optionalclaims.md) , представляют собой коллекцию **оптионалклаим**. Если это поддерживается определенным утверждением, вы также можете изменить поведение Оптионалклаим с помощью `additionalProperties` свойства.

Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|аддитионалпропертиес|Коллекция строк| Дополнительные свойства утверждения. Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве Name. |
|основы|Логический| Если задано значение true, то требование, заданное клиентом, необходимо, чтобы обеспечить гладкую авторизацию для конкретной задачи, запрашиваемой конечным пользователем. Значение по умолчанию  false.|
|name|String| Имя необязательного утверждения. |
|source|String| Источник утверждения (объект каталога). В свойствах расширения существуют предопределенные утверждения и пользовательские утверждения. Если исходное значение равно null, утверждение является предварительно определенным необязательным утверждением. Если исходное значение — User, то значение свойства Name — это свойство Extension объекта User. |

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