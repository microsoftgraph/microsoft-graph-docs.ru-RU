---
title: Тип ресурса Виндовсинформатионпротектионвипеактион
description: Представляет запросы на очистку, выданные администратором клиента для устройств Windows "применяет собственные устройства" (BYOD).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47047f401bbf0a690494490cbbd3b934340a26c9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791994"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Тип ресурса Виндовсинформатионпротектионвипеактион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет запросы на очистку, выданные администратором клиента для устройств Windows "применяет собственные устройства" (BYOD).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсинформатионпротектионвипеактионс](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|Коллекция [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Список свойств и связей объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Получение Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[Виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Чтение свойств и связей объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Создание Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[Виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|
|[Удаление Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Нет|Удаляет объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[Обновление Виндовсинформатионпротектионвипеактион](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[Виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Обновление свойств объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|status|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия очистки. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|Таржетедусерид|String|UserId, целевой для этого действия очистки.|
|Таржетеддевицерегистратионид|String|Девицерегистратионид, предназначенный для этого действия очистки.|
|Таржетеддевиценаме|String|Имя целевого устройства.|
|Таржетеддевицемакаддресс|String|Mac-адрес целевого устройства.|
|Ластчеккиндатетиме|DateTimeOffset|Время последнего возврата устройства, которое было назначено для этого действия очистки.|

## <a name="relationships"></a>Отношения
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





