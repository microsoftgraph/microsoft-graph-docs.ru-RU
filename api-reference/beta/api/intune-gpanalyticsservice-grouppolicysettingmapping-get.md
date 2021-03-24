---
title: Get groupPolicySettingMapping
description: Чтение свойств и связей объекта groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 898bfe9e7a688a753a51d3f5536962a2eb383d85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135497"
---
# <a name="get-grouppolicysettingmapping"></a>Get groupPolicySettingMapping

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1143

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
    "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
    "parentId": "Parent Id value",
    "childIdList": [
      "Child Id List value"
    ],
    "settingName": "Setting Name value",
    "settingValue": "Setting Value value",
    "settingValueType": "Setting Value Type value",
    "settingDisplayName": "Setting Display Name value",
    "settingDisplayValue": "Setting Display Value value",
    "settingDisplayValueType": "Setting Display Value Type value",
    "settingValueDisplayUnits": "Setting Value Display Units value",
    "settingCategory": "Setting Category value",
    "mdmCspName": "Mdm Csp Name value",
    "mdmSettingUri": "Mdm Setting Uri value",
    "mdmMinimumOSVersion": 3,
    "settingType": "policy",
    "isMdmSupported": true,
    "mdmSupportedState": "supported",
    "settingScope": "device",
    "intuneSettingUriList": [
      "Intune Setting Uri List value"
    ],
    "intuneSettingDefinitionId": "Intune Setting Definition Id value",
    "admxSettingDefinitionId": "Admx Setting Definition Id value"
  }
}
```




