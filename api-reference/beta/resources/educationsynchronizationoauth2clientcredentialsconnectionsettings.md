---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ffc3af93a90ba0d6991007a64d24b9fb776e8bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972371"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.

Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Токенурл** | String | URL-адрес для получения маркеров доступа для поставщика данных. |
| **scope** | String | [Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3). |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
