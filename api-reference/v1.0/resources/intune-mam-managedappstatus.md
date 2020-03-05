---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: deaca18dd8a11c930bdd052a6e3c1f94f0de1a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448328"
---
# <a name="managedappstatus-resource-type"></a>Тип ресурса managedAppStatus

Пространство имен: Microsoft. Graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет состояние защиты и конфигурации приложений для организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedAppStatus](../api/intune-mam-managedappstatus-list.md)|Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|[Получение объекта managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Понятное имя отчета о состоянии.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




