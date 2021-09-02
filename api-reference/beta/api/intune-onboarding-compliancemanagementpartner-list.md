---
title: Список complianceManagementPartners
description: Список свойств и связей объектов complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79976e827d2cf99e308626565df5bc7613ae9bc4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788537"
---
# <a name="list-compliancemanagementpartners"></a>Список complianceManagementPartners

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.complianceManagementPartner",
      "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "displayName": "Display Name value",
      "macOsOnboarded": true,
      "windowsOnboarded": true,
      "androidOnboarded": true,
      "iosOnboarded": true,
      "macOsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "windowsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
            "deviceAndAppManagementAssignmentFilterType": "include",
            "collectionId": "Collection Id value"
          }
        }
      ]
    }
  ]
}
```



