---
title: Тип ресурса managedAppPolicyDeploymentSummary
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3c740f31a5c22dc1352b3d3eec5dfa9ab8c67bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302518"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a>Тип ресурса managedAppPolicyDeploymentSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта managedAppPolicyDeploymentSummary](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).|
|[Обновление объекта managedAppPolicyDeploymentSummary](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Пока не задокументировано.|
|configurationDeployedUserCount|Int32|Пока не задокументировано.|
|lastRefreshTime|DateTimeOffset|Пока не задокументировано.|
|configurationDeploymentSummaryPerApp|Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)|Пока не задокументировано.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```




