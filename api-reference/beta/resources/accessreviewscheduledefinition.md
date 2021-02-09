---
title: Тип ресурса accessReviewScheduleDefinition
description: Представляет серию отзывов о доступе или доступе.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f95047602ec1a73549b6b5c4217e32890a5996e6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161161"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание проверки доступа Azure [AD.](accessreviewsv2-root.md) 

Объект accessReviewScheduleDefinition содержит список объектов [accessReviewInstance.](accessreviewinstance.md) Каждое повторение определения расписания создает экземпляр. Экземпляры также представляют каждую уникальную проверяемую группу. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения. В случае разовой проверки для одной группы будет создан только один экземпляр.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [Коллекция accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Перечисляет все accessReviewScheduleDefinition. Не включает связанные экземпляры accessReviewInstance в листинги. |
|[Get accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите accessReviewScheduleDefinition с указанным ид. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создайте новый accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление accessReviewScheduleDefinition с указанным идентификатором. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта accessReviewScheduleDefinition с помощью указанного идентификатора. |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| id | String | Уникальный идентификатор проверки доступа, назначенного функции.|
| displayName | String   | Название серии отзывов о доступе. Требуется при создании. |
| createdDateTime  |DateTimeOffset  | Дата и время создания серии отзывов. |
| lastModifiedDateTime | DateTimeOffset   | Дата и время последнего изменения серии отзывов.|
| status  |string   | Это поле, доступное только для чтения, указывает состояние accessReview. Типичные состояния: `Initializing` , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| descriptionForAdmins  |string  |  Описание, предоставленное создателями отзывов, чтобы предоставить администраторам дополнительный контекст проверки. |
| descriptionForReviewers |string | Описание, предоставленное авторами отзывов, чтобы предоставить рецензентам дополнительный контекст проверки. Рецензенты увидят это описание в сообщении электронной почты, отослав запрос на проверку. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший этот отзыв. |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  | Определяет область пользователей, проверяемую в группе. Поддерживаемые области [см. в accessReviewScope.](accessreviewscope.md) Требуется при создании. |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | В случае проверки всех групп это определяет область проверки групп. Каждая группа станет уникальным accessReviewInstance из серии отзывов о доступе.  Поддерживаемые области см. [в accessReviewScope.](accessreviewscope.md) | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для серии отзывов о доступе см. ниже в определении типа. |
| рецензенты   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверки доступа используется для определения проверяющих. См. [accessReviewReviewerScope.](accessreviewreviewerscope.md) Требуется при создании. |
| backupReviewers   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверяющих используется для определения списка проверяющих. Эти рецензенты будут уведомлены о необходимости принятия мер, если пользователи не найдены в списке указанных рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует или руководитель указан как рецензент, но руководитель пользователя не существует. См. [accessReviewReviewerScope.](accessreviewreviewerscope.md) |
| instances |Collection(microsoft.graph.accessReviewInstance)|  Набор экземпляров проверки доступа для этой серии отзывов о доступе. Проверки доступа, которые не повторялись, будут иметь только один экземпляр; в противном случае для каждого повторения будет иметься экземпляр. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |[Коллекция accessReviewInstance](accessreviewinstance.md)         | Если это `accessReviewScheduleDefinition` повторяющаяся проверка доступа, экземпляры представляют каждое повторение. Повторная проверка будет иметь только один экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую в `accessReviewScheduleDefinition` . Если проверка имеет несколько групп и несколько экземпляров, каждая группа будет иметь уникальный экземпляр для каждого повторения. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
