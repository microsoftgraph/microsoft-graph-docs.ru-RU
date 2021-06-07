---
title: Получить complianceManagementPartner
description: Чтение свойств и связей объекта complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bab808f9443440c673a340db877bff77b28f34c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752555"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="4eec4-103">Получить complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4eec4-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="4eec4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eec4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4eec4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4eec4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eec4-106">Чтение свойств и связей объекта [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="4eec4-106">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eec4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4eec4-107">Prerequisites</span></span>
<span data-ttu-id="4eec4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eec4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eec4-110">Permission type</span></span>|<span data-ttu-id="4eec4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eec4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eec4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eec4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4eec4-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eec4-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4eec4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eec4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eec4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eec4-115">Not supported.</span></span>|
|<span data-ttu-id="4eec4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4eec4-116">Application</span></span>|<span data-ttu-id="4eec4-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eec4-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eec4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eec4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4eec4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4eec4-119">Optional query parameters</span></span>
<span data-ttu-id="4eec4-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4eec4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eec4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eec4-121">Request headers</span></span>
|<span data-ttu-id="4eec4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eec4-122">Header</span></span>|<span data-ttu-id="4eec4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4eec4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eec4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eec4-124">Authorization</span></span>|<span data-ttu-id="4eec4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eec4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eec4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4eec4-126">Accept</span></span>|<span data-ttu-id="4eec4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4eec4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eec4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eec4-128">Request body</span></span>
<span data-ttu-id="4eec4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eec4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eec4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eec4-130">Response</span></span>
<span data-ttu-id="4eec4-131">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4eec4-131">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eec4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4eec4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eec4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eec4-133">Request</span></span>
<span data-ttu-id="4eec4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eec4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="4eec4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eec4-135">Response</span></span>
<span data-ttu-id="4eec4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eec4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1324

{
  "value": {
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
}
```




