---
title: тип ресурса roleManagement
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b454eb4e5ce477273f9a4fd7f0d373240502c02d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787232"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get roleManagement](../api/intune-rbac-rolemanagement-get.md)|[roleManagement](../resources/intune-rbac-rolemanagement.md)|Чтение свойств и связей [объекта roleManagement.](../resources/intune-rbac-rolemanagement.md)|
|[Обновление roleManagement](../api/intune-rbac-rolemanagement-update.md)|[roleManagement](../resources/intune-rbac-rolemanagement.md)|Обновление свойств объекта [roleManagement.](../resources/intune-rbac-rolemanagement.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceManagement|[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)|RbacApplication для управления устройствами|

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



