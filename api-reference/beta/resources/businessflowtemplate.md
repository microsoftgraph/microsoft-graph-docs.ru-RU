---
title: Тип ресурса businessFlowTemplate
description: В Azure AD access дается обзор компонента, `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081546"
---
# <a name="businessflowtemplate-resource-type"></a>Тип ресурса businessFlowTemplate

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.

Поток шаблон бизнес-объекты создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.  Можно создавать без дополнительных бизнес-поток шаблонов.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) коллекции| Получение шаблонов поток business подходят для доступа к обзоры.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Функция назначенный идентификатор шаблона поток business                                      |
| `displayName`            |`String`                | Имя шаблона поток business                                                             |


## <a name="relationships"></a>Связи

Нет.

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
