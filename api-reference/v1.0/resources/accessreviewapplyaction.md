---
title: тип ресурса accessReviewApplyAction
description: Представляет действия, которые необходимо принять для рассмотренных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b3ebf02cc2d5ea2c9f3ee5e64e960d2301817b9955e119a0564ce89b0ec3f9fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249337"
---
# <a name="accessreviewapplyaction-resource-type"></a>тип ресурса accessReviewApplyAction

Пространство имен: microsoft.graph

Представляет базовый класс для применения действий в [accessReviewScheduleSettings](accessreviewschedulesettings.md) [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Поддерживаемые производные типы:

- [removeAccessApplyAction](removeaccessapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на удаление доступа к объекту, проверяемого по завершении проверки. Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings и не требует указаний.

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на отключение и удаление пользователя, проверяемого по завершении проверки. Это тип по умолчанию, который должен быть указан в accessReviewScheduleSettings.

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

