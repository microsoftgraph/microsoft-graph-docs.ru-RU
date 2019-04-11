---
title: Тип ресурса Граупполиципресентатиондропдовнлист
description: Представляет элемент dropdownList и элемент enum ADMX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b70b9b5385203921151e4bc9f01c2e3a7d28cd8d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799078"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>Тип ресурса Граупполиципресентатиондропдовнлист

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент dropdownList и элемент enum ADMX.


НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатиондропдовнлистс](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|Коллекция [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Список свойств и связей объектов [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Получение Граупполиципресентатиондропдовнлист](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[Граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Чтение свойств и связей объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Создание Граупполиципресентатиондропдовнлист](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[Граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Создание нового объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Удаление Граупполиципресентатиондропдовнлист](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|Нет|Удаляет объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).|
|[Обновление Граупполиципресентатиондропдовнлист](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[Граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Обновление свойств объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Дефаултитем|[Граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.|
|items|Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|Представляет набор локализованных отображаемых имен и связанных с ними значений.|
|Обязательный|Boolean|Требование ввести значение в поле параметр. Значение по умолчанию  false.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "String",
    "value": "String"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "String",
      "value": "String"
    }
  ],
  "required": true
}
```





