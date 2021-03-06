---
title: Тип ресурса Граупполициоператион
description: Сущность представляет операцию групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff1f165c83d7d0763da320ffd33a3bd6c1dda3a1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259720"
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
|[Получение Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Чтение свойств и связей объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Создание Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Создание нового объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Удаление Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|Нет|Удаляет объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md).|
|[Обновление Граупполициоператион](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Обновление свойств объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|оператионтипе|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|Тип операции с групповой политикой. Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|оператионстатус|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|Состояние операции групповой политики. Возможные значения: `unknown`, `inProgress`, `success`, `failed`.|
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




