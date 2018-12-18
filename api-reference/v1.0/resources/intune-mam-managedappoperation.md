---
title: Тип ресурса managedAppOperation
description: Представляет операцию, примененную к регистрации приложения.
author: tfitzmac
ms.openlocfilehash: d92c467f1ff5eae403f348deac2cb6c17a3a950d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345411"
---
# <a name="managedappoperation-resource-type"></a>Тип ресурса managedAppOperation

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет операцию, примененную к регистрации приложения.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов List managedAppOperation](../api/intune-mam-managedappoperation-list.md)|Коллекция [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Получение объекта managedAppOperation](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Чтение свойств и связей объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Создание объекта managedAppOperation](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Удаление объекта managedAppOperation](../api/intune-mam-managedappoperation-delete.md)|Нет|Удаляет объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Обновление объекта managedAppOperation](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя операции.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения операции для приложения.|
|state|String|Текущее состояние операции|
|id|Строка|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Связи
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



