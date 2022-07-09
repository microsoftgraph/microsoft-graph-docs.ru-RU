---
title: Тип ресурса accessReviewApplyAction
description: Представляет действие, которое необходимо выполнить для проверяемых пользователей после завершения экземпляра проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c88cc607cedb23be344ac5bb33573dedaadb1467
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698165"
---
# <a name="accessreviewapplyaction-resource-type"></a>Тип ресурса accessReviewApplyAction

Пространство имен: microsoft.graph

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

