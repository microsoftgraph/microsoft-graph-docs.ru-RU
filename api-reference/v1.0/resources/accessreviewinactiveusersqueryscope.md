---
title: accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области обзора доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c7c0fcfb14041888ba760492bcfe6a2a224eb8656fdab8d7fee922f3e86b2af9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230825"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope

Пространство имен: microsoft.graph

Тип [accessReviewQueryScope,](../resources/accessreviewqueryscope.md) который позволяет выбирать только неактивных пользователей в области обзора доступа. Продолжительность неактивности рассчитывается на основе последней даты регистрации пользователя с датой начала проверки доступа экземпляра, как определено в свойстве параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md). 

Наследует [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inactiveDuration|Длительность|Определяет продолжительность бездействия. Неактивность основана на последнем знаке даты пользователя по сравнению с датой начала проверки доступа. Если это свойство не указано, ему назначено значение по `PT0S` умолчанию.|
|Запрос|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` . Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewInactiveUsersQueryScope** см. в рубрике Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.

## <a name="relationships"></a>Связи
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
