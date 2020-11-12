---
title: Тип ресурса Акцессревиевревиеверскопе
description: Указывает, кто будет просматривать проверку доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001059"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Тип ресурса Акцессревиевревиеверскопе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Акцессревиевревиеверскопе определяет, кто будет проверять экземпляры объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md). Он выражается в виде запроса OData, который позволяет предоставлять проверяющих как статический список пользователей (например, определенных пользователей, владельцев группы, членов группы) или динамически (например, в случае, если каждый пользователь просматривается руководителем). Чтобы создать самостоятельный обзор (где пользователи просматривают собственный доступ), не предоставляйте проверяющих при создании [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .


## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Запрос, указывающий, кто будет рецензентом. Примеры приведены в таблице. |
| куеритипе | Строка | Тип запроса. Примеры включают `MicrosoftGraph` и `ARM` . |
| куерирут | Строка | В сценарии, где Рецензенты должны быть указаны динамически, это свойство используется для указания относительного источника запроса. Это свойство необходимо только в том случае, если указан относительный запрос (например,./Манажер). |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Поддерживаемые запросы для Акцессревиевревиеверскопе

|Сценарий| Запрос | куеритипе | куерирут |
|--|--|--|--|
| Владелец группы как проверяющий | Идентификатор/граупс/{грауп}/овнерс |MicrosoftGraph||
| Определенный пользователь как проверяющий | /усерс/{Усер ID} |MicrosoftGraph||
| Руководитель пользователя, который просматривается как проверяющий | ./Манажер | MicrosoftGraph |решения|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
