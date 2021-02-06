---
title: Тип ресурса verifiedCustomDomainCertificatesMetadata
description: Представляет настраиваемые метаданные сертификата для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc0f839d91147f80d41dc48ee53c0f888aa35283
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137594"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>Тип ресурса verifiedCustomDomainCertificatesMetadata

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные сертификата настраиваемого домена для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с прокси-сервером приложения. Использование настраиваемого домена позволяет использовать для приложения собственное доменное имя вместо домена по умолчанию msappproxy.net домена. Чтобы узнать больше, [пользовательские домены в прокси приложения Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|expiryDate|DateTimeOffset| Дата окончания срока действия сертификата настраиваемого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
|issueDate|DateTimeOffset| Дата выдачи настраиваемого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
|issuerName|Строка| Имя issuer сертификата настраиваемого домена. |
|subjectName|String| Имя субъекта пользовательского сертификата домена. |
|thumbprint|Строка| Отпечаток, связанный с сертификатом пользовательского домена. |

## <a name="json-representation"></a>Представление в формате JSON

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
