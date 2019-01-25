---
title: Тип ресурса businessFlowTemplate
description: В Azure AD access дается обзор компонента, `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529581"
---
# <a name="businessflowtemplate-resource-type"></a>Тип ресурса businessFlowTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.

Поток шаблон бизнес-объекты создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.  Можно создавать без дополнительных бизнес-поток шаблонов.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) коллекции| Получение шаблонов поток business подходят для доступа к обзоры.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Функция назначенный идентификатор шаблона поток business                                      |
| `displayName`            |`String`                | Имя шаблона поток business                                                             |


## <a name="relationships"></a>Отношения

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

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
