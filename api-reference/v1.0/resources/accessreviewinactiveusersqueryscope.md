---
title: Тип ресурса accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18790d11628f7e57a349a357e46ba75377e57cc4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697577"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>Тип ресурса accessReviewInactiveUsersQueryScope

Пространство имен: microsoft.graph

Тип [accessReviewQueryScope](../resources/accessreviewqueryscope.md) , который позволяет выбирать только неактивных пользователей в области проверки доступа. Продолжительность бездействия вычисляется на основе даты последнего входа пользователя в дату начала проверки доступа, как определено в свойстве параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inactiveDuration|Длительность|Определяет длительность бездействия. Бездействие основано на дате последнего входа пользователя по сравнению с датой начала экземпляра проверки доступа. Если это свойство не указано, этому свойству назначается значение по умолчанию `PT0S`.|
|Запрос|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|Строка|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

Необходимо также указать **свойство @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope`. Дополнительные сведения о параметрах  конфигурации области с помощью **accessReviewInactiveUsersQueryScope** см. в статье "Настройка области определения проверки доступа с помощью microsoft [API Graph](/graph/accessreviews-scope-concept)".

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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
