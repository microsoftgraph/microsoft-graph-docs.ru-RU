---
title: Тип ресурса deviceManagementPartner
description: Объект, представляющий подключение к партнеру по управлению устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 94ec7345a8527d31c08873e15d6633455ac1ebbf
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734916"
---
# <a name="devicemanagementpartner-resource-type"></a>Тип ресурса deviceManagementPartner

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий подключение к партнеру по управлению устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-list.md)|Коллекция [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Получение объекта deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Создание объекта deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-create.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Удаление объекта deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-delete.md)|Нет|Удаляет объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Обновление объекта deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Тип партнерского приложения. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|Идентификатор одноклиентского приложения партнера|
|displayName|String|Отображаемое имя партнера|
|isConfigured|Boolean|Указывает, настроен ли партнер по управлению устройствами|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```





