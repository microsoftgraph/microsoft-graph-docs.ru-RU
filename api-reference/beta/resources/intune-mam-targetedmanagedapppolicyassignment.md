---
title: Тип ресурса targetedManagedAppPolicyAssignment
description: Тип развертывания групп или приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dac2ff59cd749fcf487c53817d2b2c3c160f69a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994596"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a>Тип ресурса targetedManagedAppPolicyAssignment

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип развертывания групп или приложений.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Получение объекта targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Удаление объекта targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|Нет|Удаляет объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|
|[Обновление объекта targetedManagedAppPolicyAssignment](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Идентификатор для развертывания группы или приложения|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





