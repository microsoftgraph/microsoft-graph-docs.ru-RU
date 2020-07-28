---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00e1e531ff33f28a2e63f76925cd0b4e7759696b
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434912"
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
| токенурл     | Строка | URL-адрес для получения маркеров доступа для поставщика данных.                                                                        |
| scope        | Строка | Область запроса доступа (см. [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).                          |

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
