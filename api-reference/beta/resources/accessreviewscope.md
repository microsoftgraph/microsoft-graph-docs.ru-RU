---
title: Тип ресурса Акцессревиевскопе
description: 'В функции рецензирования Access в Azure AD — `accessReviewScope` указывает, какие сущности будут проверены при проверке доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001043"
---
# <a name="accessreviewscope-resource-type"></a>Тип ресурса Акцессревиевскопе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Акцессревиевскопе** определяет, какие сущности будут проверены в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md). Он выражается в запросе OData. Тип запроса также должен быть выражен таким образом, чтобы можно было поддерживать сценарии для просмотра сущностей за преMicrosoftGraph, таких как ARM.

## <a name="properties"></a>Свойства
| Свойство   | Тип  | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос |Строка  | Запрос, указывающий, что будет рассмотрено. Примеры приведены в таблице. |
|куеритипе  |Строка | Тип запроса. Примеры включают MicrosoftGraph и ARM. |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>Поддерживаемые запросы для Акцессревиевскопе в качестве области
Ниже приведены запросы, поддерживаемые в качестве `scope` свойства в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|-- |
| Просмотр всех пользователей, назначенных группе | Идентификатор/граупс/{грауп}/Транситивемемберс ||
| Обзор гостевых пользователей, назначенных группе | /граупс/{грауп ID}/Микрософт.граф.Усер/? $count = true&$filter = (userType EQ "гость") ||
| Проверка пользователей, назначенных всем группам | ./мемберс/Микрософт.граф.Усер/? $count = true&$filter = (userType EQ "гость") | Обратите внимание, что соответствующий Инстанцеенумератионскопе также должен быть передан в Акцессревиевсчедуледефинитион. В таблице ниже представлен запрос Инстанцеенумератионскопе. |
| Проверка Ассигмент на доступ к пакету управления обслуживанием | /Идентитиговернанце/ентитлементманажемент/акцесспаккажеассигнментс? $filter = (Акцесспаккажеид EQ "{ИД пакета}" и assignmentPolicyId EQ "{ID}")| Обратите внимание, что для проверки назначений пакетов Access поддерживается только чтение|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>Поддерживаемые запросы для Акцессревиевскопе как Инстанцеенумератионскопе
Ниже приведены запросы, поддерживаемые в качестве `instanceEnumerationScope` свойства в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|--|
| Проверка пользователей, которым назначены все группы, за исключением указанных групп | /граупс? $filter = (groupTypes/Any (к:к + EQ + ' Unified ') и идентификатор Ne ' {Group ID} ' и ID Ne ' {Group ID} ' и ID Ne ' {Group ID} ') &$count = true | Обратите внимание, что соответствующая область также должна передаваться в Акцессревиевсчедуледефинитион. В разделе "Просмотр гостевых пользователей, назначенных всем группам" в таблице свойств области над запросом области. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
