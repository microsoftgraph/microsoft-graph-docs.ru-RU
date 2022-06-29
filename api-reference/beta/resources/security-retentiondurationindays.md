---
title: Тип ресурса retentionDurationInDays
description: Представляет количество дней, в течение которых элемент будет храниться до его удаления.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 4f8546d98e5430651ae672737e3d32a5e4744738
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447782"
---
# <a name="retentiondurationindays-resource-type"></a>Тип ресурса retentionDurationInDays

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет количество дней, в течение которых элемент будет храниться до его удаления.


Наследуется [от retentionDuration](../resources/security-retentionduration.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|days|Int32|Указывает период времени в днях, в течение которого будет храниться элемент с примененной меткой хранения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionDurationInDays"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionDurationInDays",
  "days": "Integer"
}
```