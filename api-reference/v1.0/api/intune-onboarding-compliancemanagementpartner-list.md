---
title: Список complianceManagementPartners
description: Список свойств и связей объектов complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a67f425e110def02b995b9fe24b218b35f28e88
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759067"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="68030-103">Список complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="68030-103">List complianceManagementPartners</span></span>

<span data-ttu-id="68030-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68030-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68030-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68030-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68030-106">Список свойств и связей объектов [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="68030-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68030-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68030-107">Prerequisites</span></span>
<span data-ttu-id="68030-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68030-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68030-110">Permission type</span></span>|<span data-ttu-id="68030-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68030-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68030-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68030-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68030-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68030-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="68030-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68030-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68030-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68030-115">Not supported.</span></span>|
|<span data-ttu-id="68030-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="68030-116">Application</span></span>|<span data-ttu-id="68030-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68030-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68030-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68030-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="68030-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68030-119">Request headers</span></span>
|<span data-ttu-id="68030-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68030-120">Header</span></span>|<span data-ttu-id="68030-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68030-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68030-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68030-122">Authorization</span></span>|<span data-ttu-id="68030-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68030-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68030-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68030-124">Accept</span></span>|<span data-ttu-id="68030-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68030-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68030-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68030-126">Request body</span></span>
<span data-ttu-id="68030-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68030-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68030-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="68030-128">Response</span></span>
<span data-ttu-id="68030-129">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68030-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68030-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68030-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="68030-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68030-131">Request</span></span>
<span data-ttu-id="68030-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68030-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="68030-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68030-133">Response</span></span>
<span data-ttu-id="68030-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68030-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.complianceManagementPartner",
      "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "displayName": "Display Name value",
      "macOsOnboarded": true,
      "androidOnboarded": true,
      "iosOnboarded": true,
      "macOsEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ]
    }
  ]
}
```




