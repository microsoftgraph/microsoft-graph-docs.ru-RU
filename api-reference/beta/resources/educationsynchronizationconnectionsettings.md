---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c82d912b13ca68dcdccd5ace0232ed65f92cd879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972492"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Тип ресурса Едукатионсинчронизатионконнектионсеттингс

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
