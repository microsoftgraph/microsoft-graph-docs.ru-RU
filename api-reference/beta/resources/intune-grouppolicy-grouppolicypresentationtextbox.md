---
title: Тип ресурса Граупполиципресентатионтекстбокс
description: Представляет элемент textBox ADMX и элемент текста ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2342dea625d4d707c9f877e5c75c75025b450c18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528047"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>Тип ресурса Граупполиципресентатионтекстбокс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент textBox ADMX и элемент текста ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионтекстбоксес](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|Коллекция [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Список свойств и связей объектов [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Получение Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Чтение свойств и связей объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Создание Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Создание нового объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Удаление Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).|
|[Обновление Граупполиципресентатионтекстбокс](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Обновление свойств объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|String|Локализованная строка по умолчанию, отображаемая в текстовом поле. По умолчанию это значение пусто.|
|Обязательный|Логический|Требование ввести значение в текстовое поле. Значение по умолчанию − ложь.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов. Значение по умолчанию — 1023.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



