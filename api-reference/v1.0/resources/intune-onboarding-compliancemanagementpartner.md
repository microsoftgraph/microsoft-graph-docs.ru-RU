---
title: тип ресурсов complianceManagementPartner
description: Партнер по управлению соответствием требованиям для всех платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d719e540747d7845a69f04c7505b8ad8bd627b8
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445733"
---
# <a name="compliancemanagementpartner-resource-type"></a>тип ресурсов complianceManagementPartner

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Партнер по управлению соответствием требованиям для всех платформ

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список complianceManagementPartners](../api/intune-onboarding-compliancemanagementpartner-list.md)|[коллекция complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Список свойств и связей объектов [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Получить complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Чтение свойств и связей объекта [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Создание complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Создание нового [объекта complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Удаление complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|Отсутствует|Удаляет [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).|
|[Обновление complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Обновление свойств объекта [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id объекта|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp последнего сердцебиения после администратора, направленного партнеру по управлению соответствием|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|String|Отображаемое имя партнера|
|macOsOnboarded|Логический|Партнер, на борту для устройств Mac.|
|AndroidOnboarded|Логический|Партнер, на борту для android-устройств.|
|iosOnboarded|Логический|Партнер, на борту для устройств ios.|
|macOsEnrollmentAssignments|[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрют устройства Mac через партнера.|
|AndroidEnrollmentAssignments|[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрют устройства Android через партнера.|
|iosEnrollmentAssignments|[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Группы пользователей, которые регистрют устройства ios через партнера.|

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



