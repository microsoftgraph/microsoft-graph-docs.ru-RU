---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d972aec91218dfc9606da4c8aa88e27b63167d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500571"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Тип ресурса Едукатионсинчронизатионконнектионсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. 

> **Примечание:** Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов параметров подключения.

## <a name="derived-types"></a>Производные типы
| Тип | Описание | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Используйте этот тип для предоставления параметров подключения OAuth1. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **clientId** | String |  Идентификатор клиента, используемый для подключения к поставщику. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к поставщику. |
