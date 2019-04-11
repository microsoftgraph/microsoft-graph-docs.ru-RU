---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 225dc4a48e0f95ccf1fdeae828c1ec603ed68802
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805826"
---
# <a name="numberrange-resource-type"></a>Тип ресурса Нумберранже

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение диапазона номеров.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Ловернумбер|Int32|Меньшее число.|
|Уппернумбер|Int32|Верхний номер.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





