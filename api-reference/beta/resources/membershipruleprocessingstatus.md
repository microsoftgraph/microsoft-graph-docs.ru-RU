---
title: тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической групповой обработки.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c86f044517ad7b808db69364413727c8d76f076
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680999"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>тип ресурса membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние динамической групповой обработки.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| status | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Текущее состояние динамической групповой обработки. Возможные значения: `NotStarted` `Running` , , , , `Succeeded` и `Failed` `UnknownFutureValue` .  <br><br> Обязательный атрибут. Только для чтения.|
| lastMembershipUpdated | edm. DateTime | Последние даты и время обновления членства в динамической группе. <br><br> Необязательно. Только для чтения.|
| errorMessage | String | Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой. <br><br> Необязательно. Только для чтения.|

### <a name="membershipruleprocessingstatusdetails-values"></a>значения membershipRuleProcessingStatusDetails

| Member | Описание |
|:-------- |:----------- |
| NotStarted | Группа была создана или обновлена и ожидает обработки.|
| Работает | Началась обработка.|
| Succeeded | Обработка завершена. Инкрементные изменения объектов обрабатываются постоянно. |
| Ошибка | Обработка столкнулась с ошибкой. Подробные сведения см. в **странице errorMessage.** |
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
