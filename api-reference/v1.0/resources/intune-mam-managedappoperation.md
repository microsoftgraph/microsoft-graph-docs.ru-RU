---
title: Тип ресурса managedAppOperation
description: Представляет операцию, примененную к регистрации приложения.
ms.openlocfilehash: 99d75983acda18e11d7abca667679eb66322dcf5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026836"
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
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

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



