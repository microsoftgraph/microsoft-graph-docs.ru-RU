---
title: тип ресурса tenantAppManagementPolicy
description: Политика по умолчанию клиента по умолчанию метода auth приложения применяет ограничения на управление приложениями.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d6ba4879df1c511e723f46d9fc9687c6ed802424
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660524"
---
# <a name="tenantappmanagementpolicy-resource-type"></a>тип ресурса tenantAppManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Политика метода проверки подлинности приложений для всех клиентов для применения ограничений управления приложениями для всех приложений и директоров служб. Эта политика применяется ко всем приложениям и директорам служб, если не переопределять при применении [appManagementPolicy](../resources/appmanagementpolicy.md) к объекту.

Наследует [от policyBase](policybase.md).

## <a name="methods"></a>Методы

| Метод                                                | Тип возвращаемых данных                                                             | Описание                                                                         |
| :---------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [Получение](../api/tenantAppManagementPolicy-get.md)       | [tenantAppManagementPolicy](../resources/tenantAppManagementPolicy.md) | Ознакомьтесь с свойствами набора политики управления приложениями по умолчанию для приложений и директоров служб. |
| [Обновление](../api/tenantAppManagementPolicy-update.md) | Нет                                                                    | Обновляет политику управления приложениями по умолчанию для приложений и директоров служб.  |

## <a name="properties"></a>Свойства

| Свойство                     | Тип                                                                     | Описание                                                           |
| :--------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| id                           | String                                                                   | Идентификатор политики по умолчанию.                                        |
| displayName                  | String                                                                   | Отображение имени политики по умолчанию. Унаследованный от [policyBase](policybase.md).                                |
| description                  | String                                                                   | Описание политики по умолчанию. Унаследованный от [policyBase](policybase.md).                                |
| isEnabled                    | Boolean                                                                  | Обозначает, включена ли политика. Значение по умолчанию — `false`.                                    |
| applicationRestrictions      | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Ограничения, которые применяются по умолчанию для всех объектов приложений в клиенте.               |
| servicePrincipalRestrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Ограничения, которые применяются по умолчанию для всех основных объектов службы в клиенте. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAppManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/tenantAppManagementPolicy",
  "id": "string (identifier)",
  "description": "string",
  "displayName": "string",
  "isEnabled": false,
  "applicationRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  }
}
```
