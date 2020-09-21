---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6a25f63c5daef72c436fe0a9a21f4d795667602
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989633"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.

Производный от [едукатионсинчронизатионконнектионсеттингс].

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | String | Идентификатор клиента, используемый для подключения к поставщику. Наследуется от [едукатионсинчронизатионконнектионсеттингс].                    |
| clientSecret | String | Секрет клиента для проверки подлинности подключения к поставщику. Наследуется от [едукатионсинчронизатионконнектионсеттингс]. |
| токенурл     | String | URL-адрес для получения маркеров доступа для поставщика данных.                                                                        |
| scope        | String | Область запроса доступа (см. [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).                          |

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md

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


