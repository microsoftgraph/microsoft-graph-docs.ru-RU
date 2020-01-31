---
title: Тип ресурса Команажементелигиблесуммарентити
description: Тип ресурса Команажементелигиблесуммарентити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636583"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a>Тип ресурса Команажементелигиблесуммарентити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние конфигурации мобильного приложения для управляемого устройства для данного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Команажементелигиблесуммарентити](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|Коллекция Команажементелигиблесуммарентити|Список свойств и связей объектов Команажементелигиблесуммарентити.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор Елигибледевицесуммарентити|
|команажедкаунт|Int32|Количество устройств, которые уже соуправлялись|
|елигиблекаунт|Int32|Количество устройств, полностью доступных для управления|
|елигиблебутнотааджоинедкаунт|Int32|Количество устройств, подходящих для управления, но еще не присоединенных к Azure Active Directory|
|нидсосупдатекаунт|Int32|Количество устройств, которые будут доступны для управления после обновления ОС|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```

