---
title: Тип ресурса Ролескопетагинфо
description: Класс, содержащий свойства объекта тега области применения роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f90ae06b56a641d18260b020588a082c2583066b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489302"
---
# <a name="rolescopetaginfo-resource-type"></a>Тип ресурса Ролескопетагинфо

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства объекта тега области применения роли.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя тега области.|
|ролескопетагид|String|Идентификатор тега Scope.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```



