---
title: Тип ресурса Граупполиципресентатионмултитекстбокс
description: Представляет элемент многоэлементного текстового поля и элемент многотекстового элемента ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce55c18c31cffeb0d63e23ef4e97412d4bbef66c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528059"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>Тип ресурса Граупполиципресентатионмултитекстбокс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент многоэлементного текстового поля и элемент многотекстового элемента ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионмултитекстбоксес](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|Коллекция [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Список свойств и связей объектов [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Получение Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Чтение свойств и связей объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Создание Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Создание нового объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Удаление Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[Обновление Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Обновление свойств объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Обязательный|Логический|Требование ввести значение в текстовое поле. Значение по умолчанию − ложь.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов. Значение по умолчанию — 1023.|
|максстрингс|Int64|Целое число без знака, задающее максимальное количество строк. Значение по умолчанию: 0.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```



