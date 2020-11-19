---
title: Тип ресурса Ролеманажемент
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9021cf7c66e3f72f11931c0a97e870294de84e0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287839"
---
# <a name="rolemanagement-resource-type"></a>Тип ресурса Ролеманажемент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Ролеманажемент](../api/intune-rbac-rolemanagement-get.md)|[ролеманажемент](../resources/intune-rbac-rolemanagement.md)|Чтение свойств и связей объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) .|
|[Обновление Ролеманажемент](../api/intune-rbac-rolemanagement-update.md)|[ролеманажемент](../resources/intune-rbac-rolemanagement.md)|Обновление свойств объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceManagement|[рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md)|Рбакаппликатион для управления устройствами|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "String (identifier)"
}
```




