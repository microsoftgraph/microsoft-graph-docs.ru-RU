---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334121"
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
