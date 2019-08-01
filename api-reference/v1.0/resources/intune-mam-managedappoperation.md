---
title: Тип ресурса managedAppOperation
description: Представляет операцию, примененную к регистрации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6653836cf21f4552e64bc433934a10b717be3708
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038026"
---
# <a name="managedappoperation-resource-type"></a>Тип ресурса managedAppOperation

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет операцию, примененную к регистрации приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов List managedAppOperation](../api/intune-mam-managedappoperation-list.md)|Коллекция [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Получение объекта managedAppOperation](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md);|Чтение свойств и связей объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Создание объекта managedAppOperation](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md);|Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Удаление объекта managedAppOperation](../api/intune-mam-managedappoperation-delete.md)|Нет|Удаляет объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Обновление объекта managedAppOperation](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя операции.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения операции для приложения.|
|state|String|Текущее состояние операции|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



