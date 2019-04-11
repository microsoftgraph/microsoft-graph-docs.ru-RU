---
title: Тип ресурса Граупполиципресентатионкомбобокс
description: Представляет элемент comboBox ADMX и элемент текста ADMX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83355dfc472945b0dd647622860d6304b01d716f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801073"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>Тип ресурса Граупполиципресентатионкомбобокс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент comboBox ADMX и элемент текста ADMX.


НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионкомбобоксес](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|Коллекция [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Список свойств и связей объектов [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Получение Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[Граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Чтение свойств и связей объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Создание Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[Граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Создание нового объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Удаление Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|Нет|Удаляет объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).|
|[Обновление Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[Граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Обновление свойств объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|String|Локализованная строка по умолчанию, отображаемая в поле со списком. По умолчанию это значение пусто.|
|мнение|Коллекция String|Локализованные строки, перечисленные в раскрывающемся списке поля со списком. По умолчанию это значение пусто.|
|Обязательный|Boolean|Указывает, следует ли указать значение для параметра. Значение по умолчанию  false.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов для параметра. Значение по умолчанию — 1023.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationComboBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "suggestions": [
    "String"
  ],
  "required": true,
  "maxLength": 1024
}
```





