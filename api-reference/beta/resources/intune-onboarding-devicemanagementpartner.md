---
title: Тип ресурса deviceManagementPartner
description: Объект, представляющий подключение к партнеру по управлению устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6806b94e559139de09ddb74a0eadc759e8e12541
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778913"
---
# <a name="devicemanagementpartner-resource-type"></a>Тип ресурса deviceManagementPartner

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

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
|id|String|Идентификатор объекта|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".|
|partnerState|[девицеманажементпартнертенантстате](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|[девицеманажементпартнерапптипе](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Тип партнерского приложения. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|String|Идентификатор одноклиентского приложения партнера|
|displayName|Строка|Отображаемое имя партнера|
|isConfigured|Boolean|Указывает, настроен ли партнер по управлению устройствами|
|вхенпартнердевицесвиллберемовед|DateTimeOffset|Дата и время в формате UTC, когда партнерские устройства будет удален. Это скоро станет обселете.|
|вхенпартнердевицесвиллбемаркедаснонкомплиант|DateTimeOffset|Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий. Это скоро станет обселете.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям|
|граупсрекуирингпартнеренроллмент|Коллекция [девицеманажементпартнерассигнмент](../resources/intune-onboarding-devicemanagementpartnerassignment.md)|Группы пользователей, указывающие, осуществляется ли регистрация через партнера.|

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
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



