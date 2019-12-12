---
title: Тип ресурса Ролеманажемент
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e19bfc30a84fc863368a7808ea1b753168ee260f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955429"
---
# <a name="rolemanagement-resource-type"></a>Тип ресурса Ролеманажемент

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
|id|Строка|Пока не задокументировано.|

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



