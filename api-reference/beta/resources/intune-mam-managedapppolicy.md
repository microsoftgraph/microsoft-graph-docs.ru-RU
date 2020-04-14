---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed9d53d683b8808ec92741d62958c0ce96fc6a55
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43372378"
---
# <a name="managedapppolicy-resource-type"></a>Тип ресурса managedAppPolicy

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|displayName|Строка|Отображаемое имя политики.|
|description|String|Описание политики.|
|createdDateTime|DateTimeOffset|Дата и время создания политики.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики.|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



