---
title: Список участников complianceManagementPartner
description: Список свойств и связей объектов complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1719a928918cd815da1af375026a7edbeb6b5802
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156898"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="63068-103">Список участников complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="63068-103">List complianceManagementPartners</span></span>

<span data-ttu-id="63068-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63068-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63068-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63068-107">Список свойств и связей объектов [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="63068-107">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63068-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63068-108">Prerequisites</span></span>
<span data-ttu-id="63068-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63068-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63068-111">Permission type</span></span>|<span data-ttu-id="63068-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63068-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63068-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="63068-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="63068-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63068-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63068-116">Not supported.</span></span>|
|<span data-ttu-id="63068-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63068-117">Application</span></span>|<span data-ttu-id="63068-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="63068-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63068-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="63068-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63068-120">Request headers</span></span>
|<span data-ttu-id="63068-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63068-121">Header</span></span>|<span data-ttu-id="63068-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63068-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63068-123">Authorization</span></span>|<span data-ttu-id="63068-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63068-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63068-125">Accept</span></span>|<span data-ttu-id="63068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63068-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63068-127">Request body</span></span>
<span data-ttu-id="63068-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63068-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63068-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63068-129">Response</span></span>
<span data-ttu-id="63068-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63068-130">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63068-131">Пример</span><span class="sxs-lookup"><span data-stu-id="63068-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63068-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="63068-132">Request</span></span>
<span data-ttu-id="63068-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63068-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="63068-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63068-134">Response</span></span>
<span data-ttu-id="63068-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63068-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




