---
title: тип ресурса accessReviewApplyAction
description: Представляет действия, которые необходимо принять для рассмотренных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82f7f88f168991ae398ca68a52e37be0baf8dec1
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60441471"
---
# <a name="accessreviewapplyaction-resource-type"></a>тип ресурса accessReviewApplyAction

Пространство имен: microsoft.graph

Представляет базовый класс для применения действий в [accessReviewScheduleSettings](accessreviewschedulesettings.md) объекта [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Поддерживаются следующие производные типы:

- [removeAccessApplyAction](removeaccessapplyaction.md) указывает на удаление доступа к объекту, проверяемого по завершении проверки. Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings и не требует указаний.

- [отключениеAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) указывает на отключение и удаление пользователя, проверяемого по завершении проверки. Это тип по умолчанию, который должен быть явно указан в accessReviewScheduleSettings.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

