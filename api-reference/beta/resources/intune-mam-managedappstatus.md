---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d144b337352222623aa5cc122b1e2d96161bd76
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994666"
---
# <a name="managedappstatus-resource-type"></a>Тип ресурса managedAppStatus

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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





