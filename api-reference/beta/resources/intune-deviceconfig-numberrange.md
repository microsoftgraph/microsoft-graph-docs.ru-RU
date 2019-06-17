---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 772ffc59bc9ac4848b6b34eee8c62f8006468784
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958720"
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





