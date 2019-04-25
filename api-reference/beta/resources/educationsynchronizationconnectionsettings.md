---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542997"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Тип ресурса Едукатионсинчронизатионконнектионсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. 

> **Примечание:** Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов параметров подключения.

## <a name="derived-types"></a>ПроизВодные типы
| Тип | Описание | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Используйте этот тип для предоставления параметров подключения OAuth1. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **clientId** | String |  Идентификатор клиента, используемый для подключения к поставщику. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к поставщику. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
