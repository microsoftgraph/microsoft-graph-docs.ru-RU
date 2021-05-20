---
title: accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области обзора доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579748"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Тип [accessReviewQueryScope,](../resources/accessreviewqueryscope.md) который позволяет выбирать только неактивных пользователей в области обзора доступа. Продолжительность неактивности рассчитывается на основе последней даты регистрации пользователя с датой начала проверки доступа экземпляра, как определено в свойстве параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md). 

Наследует [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inactiveDuration|Длительность|Определяет продолжительность бездействия. Неактивность основана на последнем знаке даты пользователя по сравнению с датой начала проверки доступа. Если это свойство не указано, ему назначено значение по `PT0S` умолчанию.|
|Запрос|Строка|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|Строка|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|Строка|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` . Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewInactiveUsersQueryScope** см. в рубрике Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
