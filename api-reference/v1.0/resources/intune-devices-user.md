---
title: Тип ресурса user
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 183c751ace228293cb20c0e459e8de75e6fb143d7e4f374e35ee2cf8a3ad884a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189527"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune-devices-user-list.md)|Коллекция объектов [user](../resources/intune-devices-user.md)|Список свойств и связей объектов [user](../resources/intune-devices-user.md).|
|[Получение пользователя](../api/intune-devices-user-get.md)|[user](../resources/intune-devices-user.md)|Чтение свойств и связей объекта [user](../resources/intune-devices-user.md).|
|[Создание пользователя](../api/intune-devices-user-create.md)|[user](../resources/intune-devices-user.md)|Создание объекта [user](../resources/intune-devices-user.md).|
|[Удаление пользователя](../api/intune-devices-user-delete.md)|Нет|Удаляет объект [user](../resources/intune-devices-user.md).|
|[Обновление пользователя](../api/intune-devices-user-update.md)|[user](../resources/intune-devices-user.md)|Обновление свойств объекта [user](../resources/intune-devices-user.md).|
|[Действие removeAllDevicesFromManagement](../api/intune-devices-user-removealldevicesfrommanagement.md)|Нет|Прекращение управления всеми устройствами для этого пользователя|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Управляемые устройства, связанные с пользователем.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




