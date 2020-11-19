---
title: Тип ресурса Граупполиципресентатионвалуелист
description: Сущность представляет коллекцию пар "имя-значение" представления списка в определении политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f95f68004cd51975635eb79c5b0de4b1712ae932
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298360"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a>Тип ресурса Граупполиципресентатионвалуелист

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет коллекцию пар "имя-значение" представления списка в определении политики.


Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуелистс](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|Коллекция [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Список свойств и связей объектов [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Получение Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Создание Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Создание нового объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|
|[Удаление Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).|
|[Обновление Граупполиципресентатионвалуелист](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Список пар для связанной презентации.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионвалуе|[граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|демонстрации|[граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Представление групповой политики, связанное со значением презентации. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

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




