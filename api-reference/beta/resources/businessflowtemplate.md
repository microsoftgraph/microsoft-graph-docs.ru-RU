---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543745"
---
# <a name="businessflowtemplate-resource-type"></a>Тип ресурса Бусинессфловтемплате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.

Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".  Невозможно создать дополнительные шаблоны бизнес-процесса.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Бусинессфловтемплатес](../api/businessflowtemplate-list.md) | Коллекция [бусинессфловтемплате](businessflowtemplate.md)| Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор шаблона рабочего процесса, назначенный компонентом                                      |
| `displayName`            |`String`                | Имя шаблона бизнес-процесса                                                             |


## <a name="relationships"></a>Связи

Нет.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Акцессревиев](../api/accessreview-create.md) | [Акцессревиев](accessreview.md) |   Создание нового Акцессревиев. |


## <a name="json-representation"></a>Представление в формате JSON

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
