---
title: Получить complianceManagementPartner
description: Чтение свойств и связей объекта complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86ae121d11003fc2b6caa5730a43b124341a232a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152690"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="59287-103">Получить complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="59287-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="59287-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59287-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59287-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59287-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59287-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59287-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59287-107">Чтение свойств и связей объекта [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="59287-107">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59287-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59287-108">Prerequisites</span></span>
<span data-ttu-id="59287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59287-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59287-111">Permission type</span></span>|<span data-ttu-id="59287-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59287-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59287-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59287-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59287-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59287-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59287-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59287-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59287-116">Not supported.</span></span>|
|<span data-ttu-id="59287-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="59287-117">Application</span></span>|<span data-ttu-id="59287-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59287-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59287-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59287-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59287-120">Optional query parameters</span></span>
<span data-ttu-id="59287-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59287-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59287-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59287-122">Request headers</span></span>
|<span data-ttu-id="59287-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59287-123">Header</span></span>|<span data-ttu-id="59287-124">Значение</span><span class="sxs-lookup"><span data-stu-id="59287-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59287-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59287-125">Authorization</span></span>|<span data-ttu-id="59287-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59287-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59287-127">Accept</span><span class="sxs-lookup"><span data-stu-id="59287-127">Accept</span></span>|<span data-ttu-id="59287-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59287-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59287-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59287-129">Request body</span></span>
<span data-ttu-id="59287-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59287-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59287-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="59287-131">Response</span></span>
<span data-ttu-id="59287-132">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59287-132">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59287-133">Пример</span><span class="sxs-lookup"><span data-stu-id="59287-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="59287-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="59287-134">Request</span></span>
<span data-ttu-id="59287-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59287-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="59287-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="59287-136">Response</span></span>
<span data-ttu-id="59287-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2390

{
  "value": {
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
}
```




