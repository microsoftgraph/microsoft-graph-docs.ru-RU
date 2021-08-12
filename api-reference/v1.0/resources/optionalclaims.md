---
title: тип optionalClaims
description: Объявляет необязательные утверждения, запрашиваемые приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 01fb75a12b27dba82066255300519cd3f830a4beeea7de77b64215170ef4f11a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180581"
---
# <a name="optionalclaims-resource-type"></a>необязательный Тип ресурсаClaims

Пространство имен: microsoft.graph объявляет необязательные требования, запрашиваемые приложением. Приложение может настраивать необязательные утверждения, которые будут возвращены в каждом из трех типов маркеров (маркер ID, маркер доступа, маркер SAML 2), которые он может получить из службы маркеров безопасности. Приложение может настроить другой набор необязательных утверждений, которые будут возвращены в каждом типе маркера. Свойство optionalClaims приложения [—](application.md) **это объект optionalClaims.**

Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт). Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|idToken|[необязательная коллекцияClaim](optionalclaim.md)| Необязательные утверждения, возвращаемые в маркере ID JWT. |
|accessToken|[необязательная коллекцияClaim](optionalclaim.md)| Необязательные утверждения, возвращаемые в маркере доступа JWT. |
|saml2Token|[необязательная коллекцияClaim](optionalclaim.md)| Необязательные утверждения, возвращаемые в маркере SAML.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
