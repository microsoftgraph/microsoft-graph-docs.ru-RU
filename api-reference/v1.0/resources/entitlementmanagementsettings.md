---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3b2e92db3119b302e280dd0f209af2e93a693c1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242702"
---
# <a name="entitlementmanagementsettings-resource-type"></a>тип ресурса entitlementManagementSettings

Пространство имен: microsoft.graph


Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-root.md)  Этот ресурс не включает параметр создателей каталога; чтобы просмотреть или изменить членство создателей каталога в роли, используйте [API](unifiedroleassignment.md) назначений ролей с поставщиком RBAC управления правами.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение entitlementManagementSettings](../api/entitlementmanagementsettings-get.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|Ознакомьтесь с свойствами объекта **entitlementManagementSettings.** |
|[Обновление entitlementManagementSettings](../api/entitlementmanagementsettings-update.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|Обновление свойств объекта **entitlementManagementSettings.** |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|durationUntilExternalUserDeletedAfterBlocked|Длительность|Если **externalUserLifecycleAction** — это продолжительность, как правило, несколько дней после блокировки внешнего пользователя до удаления учетной `blockSignInAndDelete` записи.|
|externalUserLifecycleAction|accessPackageExternalUserLifecycleAction|Автоматическое действие, которое служба должна принять при удалении последнего назначения пакета доступа внешнего пользователя. Допустимые значения: `none`, `blockSignIn`, `blockSignInAndDelete`, `unknownFutureValue`.|
|id|Строка|Константа. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSettings",
  "id": "String",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```

