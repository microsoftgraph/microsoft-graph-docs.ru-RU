---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5b0229ae431c02f85d393ff80b0bba32e32683c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334037"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При использовании [предоставления учетНых данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.

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
