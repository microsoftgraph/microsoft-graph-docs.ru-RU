---
title: тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системе знать, как подключаться к API поставщика. '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4885c2b661d2346eb80d274243c9b15d58769407
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695281"
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

Ниже приводится представление JSON этого ресурса.

<!-- {
  "blockType": "resource",
   truncated: true,
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings"
}-->

```json
{}
```
