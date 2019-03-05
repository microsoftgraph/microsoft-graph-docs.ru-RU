---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143241"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>Тип ресурса Еджехомебуттонопенскустомурл

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.


НаСледуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Хомебуттонкустомурл|String|Заданный URL-адрес для загрузки.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




