---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e03efcfdc49f41ee52c401ff7a70a8734cb3a3c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821096"
---
# <a name="managedapppolicy-resource-type"></a>Тип ресурса managedAppPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|displayName|String|Отображаемое имя политики.|
|description|String|Описание политики.|
|createdDateTime|DateTimeOffset|Дата и время создания политики.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
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



