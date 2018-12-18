---
title: Тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. '
author: mmast-msft
ms.openlocfilehash: 4e8b62a46fa6d14508a9d57ffedc46411910433d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350626"
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
| **clientId** | String. |  Идентификатор клиента, используемого для подключения к поставщику. |
| **clientSecret** | String. |  Секрет клиента для проверки подлинности подключения к поставщику. |