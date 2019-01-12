---
title: Тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f9bb19ec9c09b06dd007eb2031f3dbb176eb12d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978230"
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
| **clientId** | String |  Идентификатор клиента, используемого для подключения к поставщику. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к поставщику. |
