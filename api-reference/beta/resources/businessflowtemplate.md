---
title: Тип ресурса businessFlowTemplate (не рекомендуется)
description: В Azure AD проверки доступа объект `businesFlowTemplate` представляет Azure AD бизнес-потока. Идентификатор шаблона, например для проверки гостевых членов группы, предоставляется вызывающим объектом при создании проверки доступа.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: cfcb1cdc6997cb9b09f2f94a603a2a70c1aaf9d9
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821024"
---
# <a name="businessflowtemplate-resource-type-deprecated"></a>Тип ресурса businessFlowTemplate (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки доступа](accessreviews-root.md) **businesFlowTemplate** представляет Azure AD бизнес-потока. Идентификатор шаблона, например для проверки гостевых членов группы, предоставляется вызывающим объектом при создании проверки доступа.

Объекты шаблона бизнес-потока создаются автоматически, когда глобальный администратор подключает клиент для использования функции проверки доступа.  Шаблоны бизнес-потока включают проверки доступа к приложениям, членство в группе, членство в роли Azure AD, членство гостевых пользователей в группе и назначения гостевых пользователей приложению. Не удается создать дополнительные шаблоны бизнес-потоков.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление businessFlowTemplates](../api/businessflowtemplate-list.md) | [Коллекция businessFlowTemplate](businessflowtemplate.md)| Получите шаблоны бизнес-потока, подходящие для проверки доступа.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id                     |Строка                | Идентификатор шаблона бизнес-потока, назначаемого компонентом. Эти значения чувствительны к регистру.                                      |
| displayName            |Строка                | Имя шаблона бизнес-потока                                                             |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создайте новый accessReview. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


