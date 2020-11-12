---
title: Тип ресурса Акцессревиевсчедулесеттингс
description: В функции рецензирования Access в Azure AD `accessReviewScheduleSettings` — представляет параметры, связанные с серией проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001047"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Тип ресурса Акцессревиевсчедулесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Акцессревиевсчедулесеттингс** определяет параметры объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| маилнотификатионсенаблед|Логический | Флаг, указывающий, включены ли сообщения электронной почты.                |
| реминдернотификатионсенаблед|Логический  | Флаг, указывающий, включены ли напоминания.   |
| жустификатионрекуиредонаппровал|Логический | Флаг, указывающий, требуются ли проверяющие для предоставления обоснования для решения. |
| дефаултдеЦисионенаблед|Логический | Флаг, указывающий, включено ли решение по умолчанию или отключено, когда проверяющие не отвечают. |
| дефаултдеЦисион|Строка | Решение выбрано, если `defaultDecisionEnabled` включено. Может иметь одно из "утверждений", "deny" или "рекомендация". |
| инстанцедуратиониндайс|Int32 | Продолжительность каждого повторения проверки ( `accessReviewInstance` ) в днях. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры для периодичности. Использование стандартного объекта повторения Outlook.  |
| аутоапплидеЦисионсенаблед|Логический | Флаг, указывающий, включена ли функция автоматического применения. |
| аппляктионс|Коллекция [акцессревиеваппляктион](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживаются два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` . Поле необходимо указать только в случае `disableAndDeleteUserApplyAction` . Обратитесь к разделу [акцессревиеваппляктион](accessreviewapplyaction.md). |
| рекоммендатионсенаблед|Логический | Флаг, указывающий, включены ли рекомендации по принятию или отключены. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
