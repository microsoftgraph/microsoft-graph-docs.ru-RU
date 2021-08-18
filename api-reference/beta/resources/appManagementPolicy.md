---
title: тип ресурса appManagementPolicy
description: Политика метода auth приложения для применения ограничений управления приложениями для определенных директоров приложений или служб.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c34d9c285b4add5976603f8b9dafa4c67dd94b7d
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336872"
---
# <a name="appmanagementpolicy-resource-type"></a>тип ресурса appManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ограничения на операции по управлению приложениями для определенных приложений и директоров служб. Если этот ресурс не настроен для приложения или директора службы, ограничения по умолчанию касаются параметров объекта [tenantAppManagementPolicy.](tenantappmanagementpolicy.md)

## <a name="methods"></a>Методы

| Метод                                                         | Тип возвращаемых данных                                                                | Описание                                                                                                            |
| :------------------------------------------------------------- | :------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [Список](../api/appManagementPolicy-list.md)      | [appManagementPolicy](../resources/appManagementPolicy.md) | Возвращает список политик управления приложениями, созданных для приложений и директоров служб, а также их свойства. |
| [Create](../api/appManagementPolicy-post.md)    | [appManagementPolicy](../resources/appManagementPolicy.md) | Создает политику управления приложениями, которая может быть назначена основному объекту приложения или службы.                   |
| [Get](../api/appManagementPolicy-get.md)       | [appManagementPolicy](../resources/appManagementPolicy.md) | Получает один объект политики управления приложениями.                                                                            |
| [Обновление](../api/appManagementPolicy-update.md) | Нет                                                                       | Обновляет политику управления приложениями.                                                                                      |
| [Удаление](../api/appManagementPolicy-delete.md) | Нет                                                                       | Удаляет политику управления приложениями из коллекции политик в appManagementPolicies.                             |
| [Список применяетсяTo](../api/appManagementPolicy-list-appliesTo.md)| [appManagementPolicy](../resources/appManagementPolicy.md)|Возвращает список приложений и основных служб, к которым применяется политика. |
| [Назначение appliesTo](../api/appManagementPolicy-post-appliesTo.md)| Нет |Возвращает список приложений и основных служб, к которым применяется политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип                                                        | Описание                                                            |
| :----------- | :---------------------------------------------------------- | :--------------------------------------------------------------------- |
| id           | String                                                      | Идентификатор политики.                                                 |
| displayName  | String                                                      | Отображает имя политики. Унаследованный от [policyBase](policybase.md).                                        |
| description  | Строка                                                      | Описание политики. Унаследованный от [policyBase](policybase.md).                                         |
| isEnabled    | Boolean                                                     | Обозначает, включена ли политика.                                      |
| ограничения | [appManagementConfiguration](appManagementConfiguration.md) | Ограничения, которые применяются к основному объекту приложения или службы. |

## <a name="relationships"></a>Связи

| Связь | Тип                                  | Описание                                                                         |
| :----------- | :------------------------------------ | :---------------------------------------------------------------------------------- |
| appliesTo    | [directoryObject](directoryobject.md) | Коллекция принципов приложений и служб, к которым применяется политика. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
[
  {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies",
    "id": "string (identifier)",
    "description": "string",
    "displayName": "string",
    "isEnabled": true,
    "restrictions": {
      "@odata.type": "microsoft.graph.appManagementConfiguration"
    }
  }
]
```
