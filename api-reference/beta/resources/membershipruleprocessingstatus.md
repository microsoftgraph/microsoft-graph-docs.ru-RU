---
title: тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической групповой обработки.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 592a07abacf15300b25bfa00e9b477f9923d6c25
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586911"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>тип ресурса membershipRuleProcessingStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние динамической групповой обработки.

## <a name="properties"></a>Свойства

| Свойство              | Тип                                                                                   | Описание                                                                                                                                                                |
| :-------------------- | :------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| status                | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | Текущее состояние динамической групповой обработки. Возможные значения: `NotStarted`, , , `Succeeded`, и `Failed``UnknownFutureValue`. `Running` <br><br> Обязательный аргумент. Только для чтения. |
| lastMembershipUpdated | edm. DateTime                                                                           | Последние даты и время обновления членства в динамической группе. <br><br> Необязательно. Только для чтения.                                                                    |
| errorMessage          | Строка                                                                                 | Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой. <br><br> Необязательно. Только для чтения.                                                                        |

### <a name="membershipruleprocessingstatusdetails-values"></a>значения membershipRuleProcessingStatusDetails

| Member             | Описание                                                                     |
| :----------------- | :------------------------------------------------------------------------------ |
| NotStarted         | Группа была создана или обновлена и ожидает обработки.                     |
| Работает            | Началась обработка.                                                         |
| Succeeded          | Обработка завершена. Инкрементные изменения объектов обрабатываются постоянно. |
| Не выполнено             | Обработка столкнулась с ошибкой. **Подробные сведения см. в странице errorMessage**.                 |
| UnknownFutureValue | Поддерживает будущие значения.                                                         |

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
