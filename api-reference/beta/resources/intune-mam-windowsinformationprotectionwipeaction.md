---
title: Тип ресурса Виндовсинформатионпротектионвипеактион
description: Представляет запросы на очистку, выданные администратором клиента для устройств Windows "применяет собственные устройства" (BYOD).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4e4016f36bc4f4eb1aabc4fdb77b9555e1a1de1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524225"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Тип ресурса Виндовсинформатионпротектионвипеактион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет запросы на очистку, выданные администратором клиента для устройств Windows "применяет собственные устройства" (BYOD).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсинформатионпротектионвипеактионс](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|Коллекция [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Список свойств и связей объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Получение Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Чтение свойств и связей объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Создание Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Удаление Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Нет|Удаляет объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[Обновление Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Обновление свойств объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|status|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия очистки. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|таржетедусерид|String|UserId, целевой для этого действия очистки.|
|таржетеддевицерегистратионид|String|Девицерегистратионид, предназначенный для этого действия очистки.|
|таржетеддевиценаме|String|Имя целевого устройства.|
|таржетеддевицемакаддресс|String|Mac-адрес целевого устройства.|
|ластчеккиндатетиме|DateTimeOffset|Время последнего возврата устройства, которое было назначено для этого действия очистки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```



