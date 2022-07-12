---
title: Тип ресурса complianceManagementPartner
description: Партнер по управлению соответствием требованиям для всех платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5098c5adc788ef3c807d6fd36c29986eb9ae5c01
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736001"
---
# <a name="compliancemanagementpartner-resource-type"></a>Тип ресурса complianceManagementPartner

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Партнер по управлению соответствием требованиям для всех платформ

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-list.md)|[Коллекция complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Список свойств и связей объектов [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Получение complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Чтение свойств и связей объекта [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Создание complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Создайте объект [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Удаление complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|Нет|Удаляет объект [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).|
|[Обновление complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Обновление свойств объекта [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего пульса после подключения администратора к партнеру по управлению соответствием требованиям|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|String|Отображаемое имя партнера|
|macOsOnboarded|Логическое|Партнер, подключенный для устройств Mac.|
|androidOnboarded|Логическое|Партнер, подключенный для устройств Android.|
|iosOnboarded|Логическое|Партнер, подключенный для устройств ios.|
|macOsEnrollmentAssignments|[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрирует устройства Mac через партнера.|
|androidEnrollmentAssignments|[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрирует устройства Android через партнера.|
|iosEnrollmentAssignments|[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрирует устройства ios через партнера.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.complianceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ]
}
```





