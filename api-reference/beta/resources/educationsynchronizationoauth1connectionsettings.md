---
title: ресурс educationSynchronizationOAuth1ConnectionSettings
description: Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a73876185469ab762a08f409028880a4f7234d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989635"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>ресурс educationSynchronizationOAuth1ConnectionSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.

Производный от [едукатионсинчронизатионконнектионсеттингс].

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | String | Идентификатор клиента, используемый для подключения к поставщику. Наследуется от [едукатионсинчронизатионконнектионсеттингс].                    |
| clientSecret | String | Секрет клиента для проверки подлинности подключения к поставщику. Наследуется от [едукатионсинчронизатионконнектионсеттингс]. |

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```


