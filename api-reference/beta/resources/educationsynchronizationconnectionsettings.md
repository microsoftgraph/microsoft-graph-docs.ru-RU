---
title: Тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 17fedb5094016bd3df3bd8262390eaa7eeb37537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841771"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Тип ресурса educationSynchronizationConnectionSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. 

> **Примечание:** В данном сложном типе абстрактный. Обращайтесь к определенным типам параметров подключения из списка.

## <a name="derived-types"></a>Производные типы
| Тип | Описание | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Этот тип используется для предоставления параметров подключения OAuth1. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Этот тип используется для предоставления параметров подключения OAuth2 предоставить учетные данные клиента. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **clientId** | Строка |  Идентификатор клиента, используемого для подключения к поставщику. |
| **clientSecret** | Строка |  Секрет клиента для проверки подлинности подключения к поставщику. |
