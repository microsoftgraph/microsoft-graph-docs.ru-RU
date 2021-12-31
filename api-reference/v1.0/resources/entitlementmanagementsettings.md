---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f8ce8cdbc275ab32a5a84164716226fb6d2dddf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649699"
---
# <a name="entitlementmanagementsettings-resource-type"></a>тип ресурса entitlementManagementSettings

Пространство имен: microsoft.graph


Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-overview.md) Этот ресурс не включает параметр создателей каталога; чтобы просмотреть или изменить членство создателей каталога в роли, используйте [API](unifiedroleassignment.md) назначений ролей с поставщиком RBAC управления правами.

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

## <a name="relationships"></a>Отношения
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

