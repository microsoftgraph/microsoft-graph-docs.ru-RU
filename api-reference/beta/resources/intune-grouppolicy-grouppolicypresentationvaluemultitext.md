---
title: Тип ресурса Граупполиципресентатионвалуемултитекст
description: Сущность представляет строковое значение представления многострочного текстового поля в определении политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba837a63b984a546d7133948dd40646a62067e16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998494"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>Тип ресурса Граупполиципресентатионвалуемултитекст

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет строковое значение представления многострочного текстового поля в определении политики.


Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуемултитекстс](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|Коллекция [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Список свойств и связей объектов [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Получение Граупполиципресентатионвалуемултитекст](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[Граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Создание Граупполиципресентатионвалуемултитекст](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[Граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Создание нового объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Удаление Граупполиципресентатионвалуемултитекст](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).|
|[Обновление Граупполиципресентатионвалуемултитекст](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[Граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Обновление свойств объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Коллекция строк|Коллекция непустых строк для связанной презентации.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|Дефинитионвалуе|[Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|демонстрации|[Граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Представление групповой политики, связанное со значением презентации. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    "String"
  ]
}
```





