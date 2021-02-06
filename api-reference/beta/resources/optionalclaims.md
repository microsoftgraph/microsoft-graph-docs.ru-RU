---
title: Тип optionalClaims
description: Объявляет необязательные утверждения, запрашиваемые приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d50b514fa29cf99f22bb42238ac9d6a66126ab53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132659"
---
# <a name="optionalclaims-resource-type"></a>Тип ресурса optionalClaims

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объявляет необязательные утверждения, запрашиваемые приложением. Приложение может настроить необязательные утверждения, возвращаемые в каждом из трех типов маркеров (маркера ИД, маркера доступа, маркера SAML 2), которые оно может получить от службы маркеров безопасности. Приложение может настроить другой набор необязательных утверждений, возвращаемых в каждом типе маркера. Свойство optionalClaims приложения [является](application.md) **объектом optionalClaims.**

Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт). Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|idToken|[Коллекция optionalClaim](optionalclaim.md)| Необязательные утверждения, возвращенные в маркере JWT ID. |
|accessToken|[Коллекция optionalClaim](optionalclaim.md)| Необязательные утверждения, возвращенные в маркере доступа JWT. |
|saml2Token|[Коллекция optionalClaim](optionalclaim.md)| Необязательные утверждения, возвращенные в маркере SAML.|

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
