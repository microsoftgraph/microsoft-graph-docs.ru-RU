---
title: Тип ресурса Граупполиципресентатионмултитекстбокс
description: Представляет элемент многоэлементного текстового поля и элемент многотекстового элемента ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e564b08aa13696993c68e611171d760baae184c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964922"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>Тип ресурса Граупполиципресентатионмултитекстбокс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент многоэлементного текстового поля и элемент многотекстового элемента ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионмултитекстбоксес](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|Коллекция [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Список свойств и связей объектов [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Получение Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[Граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Чтение свойств и связей объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Создание Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[Граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Создание нового объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Удаление Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[Обновление Граупполиципресентатионмултитекстбокс](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[Граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Обновление свойств объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Обязательный|Boolean|Требование ввести значение в текстовое поле. Значение по умолчанию − ложь.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов. Значение по умолчанию — 1023.|
|Максстрингс|Int64|Целое число без знака, задающее максимальное количество строк. Значение по умолчанию: 0.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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





