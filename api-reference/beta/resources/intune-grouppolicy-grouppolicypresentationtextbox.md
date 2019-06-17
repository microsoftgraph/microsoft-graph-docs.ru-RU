---
title: Тип ресурса Граупполиципресентатионтекстбокс
description: Представляет элемент textBox ADMX и элемент текста ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08edce84569edb8bd85261b0796aaa3e6a5b1eb6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964838"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>Тип ресурса Граупполиципресентатионтекстбокс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент textBox ADMX и элемент текста ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионтекстбоксес](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|Коллекция [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Список свойств и связей объектов [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Получение Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[Граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Чтение свойств и связей объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Создание Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[Граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Создание нового объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Удаление Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).|
|[Обновление Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[Граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Обновление свойств объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|String|Локализованная строка по умолчанию, отображаемая в текстовом поле. По умолчанию это значение пусто.|
|Обязательный|Boolean|Требование ввести значение в текстовое поле. Значение по умолчанию − ложь.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов. Значение по умолчанию — 1023.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "required": true,
  "maxLength": 1024
}
```





