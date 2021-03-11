---
title: verifiedCustomDomainCertificatesMetadata resource type
description: Представляет настраиваемые метаданные сертификации для локального приложения, опубликованного с помощью прокси-сервера приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: eab6823bdd3ed6a822cbeabdebf0aedfb654b769
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721434"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>verifiedCustomDomainCertificatesMetadata resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемые метаданные сертификата домена для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с помощью прокси-приложения. Использование настраиваемого домена позволяет использовать собственное доменное имя вместо домена по умолчанию, msappproxy.net, для приложения. Дополнительные дополнительные новости см. в [специально созданных доменах в Прокси-сервере приложений Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|expiryDate|DateTimeOffset| Срок действия пользовательского сертификата домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|issueDate|DateTimeOffset| Дата выпуска настраиваемого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|issuerName|String| Имя эмитента пользовательского сертификата домена. |
|subjectName|String| Имя субъекта пользовательского сертификата домена. |
|отпечатки пальцев|String| Отпечатки пальцев, связанные с пользовательским сертификатом домена. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
