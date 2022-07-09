---
title: Тип ресурса accessReviewApplyAction
description: Представляет действие, которое необходимо выполнить для проверяемых пользователей после завершения экземпляра проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aed70bb75bd690ec8532727b90954b23e927f16e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697255"
---
# <a name="accessreviewapplyaction-resource-type"></a>Тип ресурса accessReviewApplyAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет базовый класс для действий применения в [accessReviewScheduleSettings](accessreviewschedulesettings.md) объекта [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . Поддерживаются следующие производные типы:

- [RemoveAccessApplyAction](removeaccessapplyaction.md) означает удаление доступа к сущности, проверяемой по завершении проверки. Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings, и его не нужно указать.

- [DisableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) указывает на отключение и удаление пользователя, проверяемого по завершении проверки. Этот тип не является типом по умолчанию и должен быть явно указан в accessReviewScheduleSettings.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON
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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
