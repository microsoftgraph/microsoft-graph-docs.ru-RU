---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d38853e40d8f88bf4aa8323395848185793cc42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500095"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.

Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **токенурл** | String | URL-адрес для получения маркеров доступа для поставщика данных. |
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
