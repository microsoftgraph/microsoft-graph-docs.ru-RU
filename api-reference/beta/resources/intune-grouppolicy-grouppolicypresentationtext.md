---
title: Тип ресурса Граупполиципресентатионтекст
description: Представляет элемент текста ADMX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2021108ef033e1529911de57be24612935896d22
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142863"
---
# <a name="grouppolicypresentationtext-resource-type"></a>Тип ресурса Граупполиципресентатионтекст

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент текста ADMX.


НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионтекстс](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|Коллекция [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Список свойств и связей объектов [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Получение Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[Граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Чтение свойств и связей объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Создание Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[Граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Создание нового объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Удаление Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Нет|Удаляет объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Обновление Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[Граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Обновление свойств объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. Значение по умолчанию — пустое значение. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|definition|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




