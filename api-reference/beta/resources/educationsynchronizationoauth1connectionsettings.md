---
title: ресурс educationSynchronizationOAuth1ConnectionSettings
description: Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 525809121b07616c6eb5077f1b12d5b736586065
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434923"
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
