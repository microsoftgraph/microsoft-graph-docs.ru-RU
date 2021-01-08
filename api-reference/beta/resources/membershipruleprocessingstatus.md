---
title: Тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической обработки группы.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864cbd9ea446655c2a0d5f950b28fa6421d2241c
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784890"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>Тип ресурса membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние динамической обработки группы.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| status | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Текущее состояние динамической обработки группы. Возможные значения: `NotStarted` , , , , и `Running` `Succeeded` `Failed` `UnknownFutureValue` .  <br><br> Обязательный. Только для чтения.|
| lastMembershipUpdated | edm. DateTime | Самая новая дата и время обновления членства в динамической группе. <br><br> Необязательно. Только для чтения.|
| errorMessage | String | Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой. <br><br> Необязательно. Только для чтения.|

### <a name="membershipruleprocessingstatusdetails-values"></a>значения membershipRuleProcessingStatusDetails

| Member | Описание |
|:-------- |:----------- |
| NotStarted | Группа создана или обновлена и ожидает обработки.|
| Выполняется | Обработка запущена.|
| Succeeded | Обработка завершена. Добавочные изменения объектов обрабатываются бессрочно. |
| Не выполнено | При обработке произошла ошибка. Подробные **сведения см. в errorMessage.** |
| UnknownFutureValue | Поддерживает будущие значения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```
