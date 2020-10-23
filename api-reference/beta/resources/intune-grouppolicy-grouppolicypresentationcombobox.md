---
title: Тип ресурса Граупполиципресентатионкомбобокс
description: Представляет элемент comboBox ADMX и элемент текста ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bea4b64b8926adcb64b4de5e1b590329b5145593
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684696"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>Тип ресурса Граупполиципресентатионкомбобокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент comboBox ADMX и элемент текста ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионкомбобоксес](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|Коллекция [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Список свойств и связей объектов [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Получение Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Чтение свойств и связей объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Создание Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Создание нового объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Удаление Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|Нет|Удаляет объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).|
|[Обновление Граупполиципресентатионкомбобокс](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Обновление свойств объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|Строка|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|Строка|Локализованная строка по умолчанию, отображаемая в поле со списком. По умолчанию это значение пусто.|
|мнение|Коллекция строк|Локализованные строки, перечисленные в раскрывающемся списке поля со списком. По умолчанию это значение пусто.|
|Обязательный|Логический|Указывает, следует ли указать значение для параметра. Значение по умолчанию  false.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов для параметра. Значение по умолчанию — 1023.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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





