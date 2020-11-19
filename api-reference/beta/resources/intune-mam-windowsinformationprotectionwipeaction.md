---
title: Тип ресурса Виндовсинформатионпротектионвипеактион
description: Представляет запросы на очистку, выданные администратором клиента для устройств Windows "применяет собственные устройства" (BYOD).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d915bfe59bf677accfaf16df8765b6c7da882cf9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302476"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Тип ресурса Виндовсинформатионпротектионвипеактион

Пространство имен: microsoft.graph

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




