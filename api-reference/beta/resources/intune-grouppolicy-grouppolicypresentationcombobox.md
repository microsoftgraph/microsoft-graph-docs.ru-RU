---
title: тип ресурса groupPolicyPresentationComboBox
description: Представляет элемент comboBox ADMX и текстовый элемент ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d431d96d3747ce1d9ea764ca924c596391224fa3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58810269"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>тип ресурса groupPolicyPresentationComboBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент comboBox ADMX и текстовый элемент ADMX.


Наследует [от groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationComboBoxes](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[коллекция groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Список свойств и связей объектов [groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Get groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Чтение свойств и связей объекта [groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Создание groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Создайте новый [объект groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Удаление groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|Нет|Удаляет [группуPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).|
|[Update groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Обновление свойств объекта [groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|Строка|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Строка|Локализованная строка по умолчанию, отображаемая в поле комбо. По умолчанию это значение пусто.|
|предложения|Коллекция String|Локализованные строки, перечисленные в выпадаемом списке комбо-окна. По умолчанию это значение пусто.|
|обязательно|Логический|Указывает, должно ли значение быть задано для параметра. Значение по умолчанию  false.|
|maxLength|Int64|Неподписаный целый ряд, который указывает максимальное количество текстовых символов для параметра. Значение по умолчанию — 1023.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



