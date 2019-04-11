---
title: Тип ресурса Девицеандаппманажементассигнедроледетаилс
description: Набор определений ролей и наЗначений ролей, назначенных пользователю.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771406"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>Тип ресурса Девицеандаппманажементассигнедроледетаилс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Набор определений ролей и наЗначений ролей, назначенных пользователю.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Роледефинитионидс|Коллекция String|Идентификаторы определений ролей для определений ролей частности, назначенных пользователю.|
|Ролеассигнментидс|Коллекция String|Идентификаторы назначения ролей для наЗначений ролей частности, назначенных пользователю.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```





