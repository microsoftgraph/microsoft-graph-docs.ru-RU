---
title: Тип ресурса Граупполиципресентатионвалуелист
description: Сущность представляет коллекцию пар "имя-значение" представления списка в определении политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4efb34c0f725c7253f30a04ba606ce5cf27a669
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998529"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a>Тип ресурса Граупполиципресентатионвалуелист

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет коллекцию пар "имя-значение" представления списка в определении политики.


Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуелистс](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|Коллекция [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Список свойств и связей объектов [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Получение Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[Граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Создание Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[Граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Создание нового объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Удаление Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).|
|[Обновление Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[Граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Список пар для связанной презентации.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```





