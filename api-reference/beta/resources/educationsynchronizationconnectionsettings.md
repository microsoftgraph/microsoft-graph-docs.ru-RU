---
title: тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системе знать, как подключаться к API поставщика. '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: eca233d7e375991f34bdd2b44351fe75f371fee1
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290590"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>тип ресурса educationSynchronizationConnectionSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры подключения поставщика. Это позволяет системе знать, как подключаться к API поставщика.

> [!NOTE]
> Этот сложный тип абстрактный. Обратитесь к указанным типам параметров подключения.

## <a name="derived-types"></a>Производные типы

| Тип                                                                                                                                      | Описание                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | Этот тип используется для предоставления параметров подключения OAuth1.                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Используйте этот тип для предоставления параметров подключения КБ OAuth2 для предоставления клиентских учетных данных. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | String | ID клиента, используемый для подключения к поставщику.                    |
| clientSecret | String | Секрет клиента для проверки подлинности подключения к поставщику. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление этого ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
  "clientId": "String",
  "clientSecret": "String",
}
```