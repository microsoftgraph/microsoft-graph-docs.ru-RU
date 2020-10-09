---
title: Тип ресурса Верифиедкустомдомаинцертификатесметадата
description: Представляет настраиваемые метаданные сертификат для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f3dc4cbe1a68ae6f7c751c9b305f95901928d17
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402954"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a>Тип ресурса Верифиедкустомдомаинцертификатесметадата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные пользовательских сертификатов домена для ресурса [онпремисеспублишинг](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения. Использование пользовательского домена позволяет использовать собственное доменное имя вместо домена по умолчанию (msappproxy.net) для вашего приложения. Дополнительные сведения см. в разделе " [Настраиваемые домены" прокси-сервера приложений Azure AD](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|експиридате|DateTimeOffset| Дата истечения срока действия сертификата настраиваемого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
|иссуедате|DateTimeOffset| Дата выпуска настраиваемого домена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
|иссуернаме|String| Имя поставщика сертификата настраиваемого домена. |
|subjectName|String| Имя субъекта пользовательского сертификата домена. |
|отпечаток|String| Отпечаток, связанный с пользовательским сертификатом домена. |

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