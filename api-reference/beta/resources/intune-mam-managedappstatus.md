---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6df9c36f15e3e20389dfc46d306b896c3fe77b5b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799148"
---
# <a name="managedappstatus-resource-type"></a>Тип ресурса managedAppStatus

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет состояние защиты и конфигурации приложений для организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppStatus](../api/intune-mam-managedappstatus-list.md)|Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|[Get managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Понятное имя отчета о состоянии.|
|id|String|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Отношения
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





