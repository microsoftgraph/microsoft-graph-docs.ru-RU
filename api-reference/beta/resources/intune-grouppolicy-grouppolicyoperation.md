---
title: Тип ресурса Граупполициоператион
description: Сущность представляет операцию групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69ab3503d761052ba8293b9133f43204a6afd7b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376919"
---
# <a name="grouppolicyoperation-resource-type"></a>Тип ресурса Граупполициоператион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет операцию групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициоператионс](../api/intune-grouppolicy-grouppolicyoperation-list.md)|Коллекция [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md)|Список свойств и связей объектов [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Получение Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md)|Чтение свойств и связей объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Создание Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md)|Создание нового объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Удаление Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|Нет|Удаляет объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md).|
|[Обновление Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md)|Обновление свойств объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|оператионтипе|[граупполициоператионтипе](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|Тип операции с групповой политикой. Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|оператионстатус|[граупполициоператионстатус](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|Состояние операции групповой политики. Возможные значения: `unknown`, `inProgress`, `success`, `failed`.|
|статусдетаилс|String|Сведения о состоянии операции групповой политики.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



