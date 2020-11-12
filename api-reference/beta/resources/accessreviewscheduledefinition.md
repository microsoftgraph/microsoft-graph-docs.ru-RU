---
title: Тип ресурса Акцессревиевсчедуледефинитион
description: Представляет серию проверки доступа или проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8ee04dde7ee19d24be5de58237f08b4fb538e8c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001042"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Тип ресурса Акцессревиевсчедуледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание [проверки доступа](accessreviewsv2-root.md)Azure AD. 

Объект Акцессревиевсчедуледефинитион содержит список объектов [акцессревиевинстанце](accessreviewinstance.md) . Каждый повтор определения расписания создаст экземпляр. Экземпляры также представляют каждую проверяемую группу. Если в определении расписания просматриваются несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения. В случае одноразового рассмотрения для каждой группы будет создан только один экземпляр.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Акцессревиевсчедуледефинитионс](../api/accessreviewscheduledefinition-list.md) | Коллекция [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Перечисление всех Акцессревиевсчедуледефинитион. Не включает связанные экземпляры Акцессревиевинстанце в вхождениях. |
|[Получение Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-get.md) | [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Получение Акцессревиевсчедуледефинитион с указанным идентификатором. |
|[Создание Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-create.md) | [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Создание нового Акцессревиевсчедуледефинитион. |
|[Удаление Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление объекта Акцессревиевсчедуледефинитион с указанным идентификатором. |
|[Обновление Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта Акцессревиевсчедуледефинитион с указанным идентификатором. |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| id | Строка | Уникальный идентификатор проверки доступа, назначенный компоненту.|
| displayName | Строка   | Имя серии проверки доступа. Требуется при создании. |
| createdDateTime  |DateTimeOffset  | Дата и время создания серии проверки. |
| lastModifiedDateTime | DateTimeOffset   | Дата и время последнего изменения ряда проверки.|
| status  |string   | В этом поле, доступном только для чтения, указывается состояние Акцессревиев. Типичные состояния:,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` , `AutoReviewing` и `AutoReviewed` . |
| дескриптионфорадминс  |строка  |  Описание, предоставленное авторами рецензирования, для предоставления более подробного контекста просмотра администраторам. |
| дескриптионфорревиеверс |строка | Описание, предоставленное авторами рецензирования, для предоставления более подробного контекста проверки рецензентам. Проверяющие увидят это описание в отправленном им сообщении электронной почты с запросом на проверку. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший эту проверку. |
| scope  |[акцессревиевскопе](../resources/accessreviewscope.md)  | Определяет область пользователей, проверенных в группе. Поддерживаемые области приведены в разделе [акцессревиевскопе](accessreviewscope.md). Требуется при создании. |
| инстанцеенумератионскопе|[акцессревиевскопе](../resources/accessreviewscope.md)  | В случае проверки всех групп это определяет область, в которой будут проверяться группы. Каждая группа станет уникальной Акцессревиевинстанце серии проверки доступа.  Поддерживаемые области приведены в разделе [акцессревиевскопе](accessreviewscope.md). | 
| settings  |[акцессревиевсчедулесеттингс](../resources/accessreviewschedulesettings.md)| Параметрах серии проверки доступа можно узнать в статье Type Definition ниже. |
| обсужден   |Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверки доступа используется, чтобы определить, кто является рецензентами. Обратитесь к разделу [акцессревиевревиеверскопе](accessreviewreviewerscope.md). Требуется при создании. |
| баккупревиеверс   |Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md)| Эта коллекция областей рецензентов используется для определения списка резервных рецензентов. Эти резервные проверяющие будут получать уведомления о предпринимаемых действиях, если в списке указанных рецензентов не найдено ни одного пользователя. Это может произойти, если владелец группы указан как проверяющий, но владелец группы не существует или руководитель указан как проверяющий, но не существует руководителя пользователя. Обратитесь к разделу [акцессревиевревиеверскопе](accessreviewreviewerscope.md). |
| instances |Collection (Microsoft. Graph. Акцессревиевинстанце)|  Набор рецензированных экземпляров Access для этого ряда проверки доступа. Для неповторяющихся просмотров необходим только один экземпляр; в противном случае будет использоваться экземпляр каждого повторения. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |Коллекция [акцессревиевинстанце](accessreviewinstance.md)         | Если это `accessReviewScheduleDefinition` повторяющаяся проверка доступа, экземпляры представляют каждое повторение. Проверка, которая не повторяется, будет иметь ровно один экземпляр. Экземпляры также представляют каждую уникальную группу в разделе "Рецензирование" в `accessReviewScheduleDefinition` . Если у рецензирования несколько групп и несколько экземпляров, каждая группа будет иметь уникальный экземпляр для каждого повторения. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "",
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
