---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f16f883622ace795628d7c34214cc4b5d12017e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989797"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>Тип ресурса Еджехомебуттонопенскустомурл

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.


Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)

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





