---
title: тип ресурса groupPolicyPresentationLongDecimalTextBox
description: Представляет элемент ADMX longDecimalTextBox и элемент ADMX longDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d3756debc5cccf71bf271356545e9c345cec96775849558df1daa5a6ec4c57a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236012"
---
# <a name="grouppolicypresentationlongdecimaltextbox-resource-type"></a>тип ресурса groupPolicyPresentationLongDecimalTextBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент ADMX longDecimalTextBox и элемент ADMX longDecimal.


Наследует [от groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationLongDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-list.md)|[коллекция groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Список свойств и связей объектов [groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Get groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-get.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Чтение свойств и связей объекта [groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Создание groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-create.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Создайте новый [объект groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Удаление groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-delete.md)|Нет|Удаляет [группуPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).|
|[Update groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-update.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Обновление свойств объекта [groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|String|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Неподписаный полный ящик, который указывает начальное значение десятичной текстовой коробки. Значение по умолчанию равно 1.|
|spin|Логический|Если верно, создайте управление спином; в противном случае создайте текстовое поле для числовой записи. Значение по умолчанию: true.|
|spinStep|Int64|Неподписавая часть, указывляемая на приращение изменений для управления спином. Значение по умолчанию равно 1.|
|обязательно|Логический|Требование ввести значение в поле параметра. Значение по умолчанию  false.|
|minValue|Int64|Неподписаный длинный, который указывает минимально допустимые значения. Значение по умолчанию равно 0.|
|maxValue|Int64|Неподписаное длинное значение, которое указывает максимально допустимые значения. Значение по умолчанию — 9999.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationLongDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```




