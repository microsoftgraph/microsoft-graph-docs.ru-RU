---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 461fe34e0d572f910f15df9521d54660f0568ad1
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703793"
---
# <a name="businessflowtemplate-resource-type"></a>Тип ресурса Бусинессфловтемплате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.

Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".  Шаблоны бизнес-процесса включают в себя обзоры разрешений на доступ к приложениям, членству в группах, членстве в роли Azure AD, членстве гостей в группе и назначения гостевых пользователей приложению. Невозможно создать дополнительные шаблоны бизнес-процесса.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Бусинессфловтемплатес](../api/businessflowtemplate-list.md) | Коллекция [бусинессфловтемплате](businessflowtemplate.md)| Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор шаблона рабочего процесса, назначенный компонентом. Эти значения вводятся с учетом регистра.                                      |
| `displayName`            |`String`                | Имя шаблона бизнес-процесса                                                             |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Акцессревиев](../api/accessreview-create.md) | [акцессревиев](accessreview.md) |   Создание нового Акцессревиев. |


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
