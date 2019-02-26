---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251169"
---
# <a name="managedapppolicy-resource-type"></a>Тип ресурса managedAppPolicy

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedAppPolicy](../api/intune-mam-managedapppolicy-list.md)|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|[Получение объекта managedAppPolicy](../api/intune-mam-managedapppolicy-get.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|[Действие targetApps](../api/intune-mam-managedapppolicy-targetapps.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики.|
|description|String|Описание политики.|
|createdDateTime|DateTimeOffset|Дата и время создания политики.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики.|
|id|String|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Связи
None

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



