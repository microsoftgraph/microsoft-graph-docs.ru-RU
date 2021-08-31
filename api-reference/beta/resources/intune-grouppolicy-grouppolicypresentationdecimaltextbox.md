---
title: тип ресурса groupPolicyPresentationDecimalTextBox
description: Представляет элемент десятичной коробки ADMX и десятичной элемент ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79ef120bf7845d95e5cbc1aa8c465a38fc3f4ee2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802959"
---
# <a name="grouppolicypresentationdecimaltextbox-resource-type"></a>тип ресурса groupPolicyPresentationDecimalTextBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент десятичной коробки ADMX и десятичной элемент ADMX.


Наследует [от groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-list.md)|[коллекция groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Список свойств и связей объектов [groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|
|[Get groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-get.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Чтение свойств и связей объекта [groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|
|[Создание groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-create.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Создайте новый [объект groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|
|[Удаление groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-delete.md)|Нет|Удаляет [группуPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).|
|[Update groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-update.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Обновление свойств объекта [groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|Строка|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Неподписаный полный ящик, который указывает начальное значение десятичной текстовой коробки. Значение по умолчанию равно 1.|
|spin|Логический|Если верно, создайте управление спином; в противном случае создайте текстовое поле для числовой записи. Значение по умолчанию: true.|
|spinStep|Int64|Неподписавая часть, указывляемая на приращение изменений для управления спином. Значение по умолчанию равно 1.|
|обязательно|Boolean|Требование ввести значение в поле параметра. Значение по умолчанию  false.|
|minValue|Int64|Неподписаный пустяк, который указывает минимально допустимые значения. Значение по умолчанию равно 0.|
|maxValue|Int64|Неподписаный пустяк, который указывает максимально допустимые значения. Значение по умолчанию — 9999.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
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



