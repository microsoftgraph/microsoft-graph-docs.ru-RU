---
title: тип ресурса businessFlowTemplate
description: В функции обзоров доступа Azure AD представляет шаблон бизнес-потока `businesFlowTemplate` Azure AD. Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 95a2723ee20777989ed1576d02c69adc649555ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433147"
---
# <a name="businessflowtemplate-resource-type"></a>тип ресурса businessFlowTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](accessreviews-root.md) представляет шаблон бизнес-потока `businesFlowTemplate` Azure AD. Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.

Объекты шаблона бизнес-потока автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.  Шаблоны бизнес-потока включают обзоры доступа к назначениям для приложения, членство в группе, членство в роли Azure AD, членство гостей в группе и назначения гостевых пользователей приложению. Дополнительные шаблоны бизнес-потока создаваться не могут.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [коллекция businessFlowTemplate](businessflowtemplate.md)| Получите шаблоны бизнес-потока, подходящие для доступа к отзывам.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор шаблона бизнес-потока, назначенного функцией. Эти значения чувствительны к делу.                                      |
| `displayName`            |`String`                | Имя шаблона бизнес-потока                                                             |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создание нового accessReview. |


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


