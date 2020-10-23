---
title: Тип ресурса Ролеманажемент
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ef912731b05fb8c4fa83aac77f7879cc9e3d7f7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725185"
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
|id|Строка|Н/Д|

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





