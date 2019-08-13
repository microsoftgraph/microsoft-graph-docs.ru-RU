---
title: Тип ресурса Граупполиципресентатионтекст
description: Представляет элемент текста ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 593169c11d09a5ef801014015a3c787333351fdc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331310"
---
# <a name="grouppolicypresentationtext-resource-type"></a>Тип ресурса Граупполиципресентатионтекст

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент текста ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионтекстс](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|Коллекция [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Список свойств и связей объектов [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Получение Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Чтение свойств и связей объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Создание Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Создание нового объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Удаление Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Нет|Удаляет объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Обновление Граупполиципресентатионтекст](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Обновление свойств объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



