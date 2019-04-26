---
title: Тип ресурса mobileAppAssignment
description: Класс, содержащий свойства, которые используются для назначения групп в мобильном приложении.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f3faff8a04709788e415b72013e32a850889ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557959"
---
# <a name="mobileappassignment-resource-type"></a>Тип ресурса mobileAppAssignment

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения групп в мобильном приложении.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppAssignment](../api/intune-apps-mobileappassignment-list.md)|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Получение объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Создание объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Удаление объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-delete.md)|Нет|Удаляет объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Обновление объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|Параметры целевого назначения, определенные администратором.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



