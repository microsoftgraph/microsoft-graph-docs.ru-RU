---
title: Тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической обработки группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f59f5f89c3aad8312504c62b29a0dbd490a37ac5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128277"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>Тип ресурса membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние динамической обработки группы.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| status | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Текущее состояние динамической обработки группы. Возможные значения: `NotStarted` , , , , и `Running` `Succeeded` `Failed` `UnknownFutureValue` .  <br><br> Обязательный элемент. Только для чтения.|
| lastMembershipUpdated | edm. DateTime | Самая новая дата и время обновления членства в динамической группе. <br><br> Необязательно. Только для чтения.|
| errorMessage | Строка | Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой. <br><br> Необязательно. Только для чтения.|

### <a name="membershipruleprocessingstatusdetails-values"></a>значения membershipRuleProcessingStatusDetails

| Member | Описание |
|:-------- |:----------- |
| NotStarted | Группа создана или обновлена и ожидает обработки.|
| Выполняется | Обработка запущена.|
| Succeeded | Обработка завершена. Добавочные изменения объектов обрабатываются бессрочно. |
| Не выполнено | При обработке произошла ошибка. Подробные **сведения см. в errorMessage.** |
| UnknownFutureValue | Поддерживает будущие значения. |

## <a name="json-representation"></a>Представление в формате JSON

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
