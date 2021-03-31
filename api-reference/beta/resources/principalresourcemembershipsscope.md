---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет для областей выбора просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2ac3dd53223b9260c3f51c3c872d36b044e698d5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469790"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>тип ресурса principalResourceMembershipsScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

PrincipalResourceMembershipsScope — это тип [accessReviewScope,](accessreviewscope.md) который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и просмотреть доступ выбранных директоров к выбранным ресурсам. См. поддерживаемые запросы, чтобы узнать, что можно выбрать. Он используется в качестве `scope` свойства [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|principalScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области, включаемые в обзор доступа.|
|resourceScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области ресурсов, для которых будет рассмотрен доступ.|

## <a name="relationships"></a>Связи
Отсутствуют.

### <a name="supported-queries-for-resourcescope"></a>Поддерживаемые запросы для resourceScope
Запросы поддерживаются как `resourceScope` свойство. Они определяют, к каков набор доступа к ресурсам. 

|Сценарий| запрос resourceScope | 
|--|--|
| Проверка доступа principalScopes к основной службе | /servicePrincipals/{service principal ID} |
| Просмотр доступа principalScopes к роли каталога Azure AD | /roleManagement/directory/roleDefinitions/{role ID} |
| Просмотр доступа principalScopes ко всем ролям каталога Azure AD | /roleManagement/directory/roleDefinitions |

### <a name="supported-queries-for-principalscope"></a>Поддерживаемые запросы для principalScope
Запросы поддерживаются как `principalScope` свойство. Они определяют набор директоров, доступ которых к связанному ресурсуScope будет рассмотрен. В связанном типе principalScope перечислены типы запросов odata, принятые в качестве principalScope.

|Сценарий| запрос principalScope | Тип запроса OData | Дополнительные комментарии |
|--|--|-- | --|
| Просмотр доступа всех пользователей к ресурсуScope | /users |[accessReviewQueryScope](accessreviewqueryscope.md)||
| Просмотр доступа гостевых пользователей к ресурсуScope | /users?$filter=(userType eq 'Guest') |[accessReviewQueryScope](accessreviewqueryscope.md)||
| Просмотр доступа всех неактивных пользователей к ресурсуScope | /users |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| Должно включать `instanceDuration` свойство|
| Просмотр доступа неактивных пользователей гостей к ресурсуScope | /users?$filter=(userType eq 'Guest') |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| Должно включать `instanceDuration` свойство|




## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
