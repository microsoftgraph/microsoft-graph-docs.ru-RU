---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9bc66171f972debe38127b70c92e7deb7a38ade
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751477"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="9bf97-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9bf97-103">List enrollmentConfigurationAssignments</span></span>

<span data-ttu-id="9bf97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bf97-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bf97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf97-106">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9bf97-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf97-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9bf97-107">Prerequisites</span></span>
<span data-ttu-id="9bf97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf97-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bf97-110">Permission type</span></span>|<span data-ttu-id="9bf97-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bf97-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bf97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf97-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf97-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9bf97-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bf97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf97-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bf97-115">Not supported.</span></span>|
|<span data-ttu-id="9bf97-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9bf97-116">Application</span></span>|<span data-ttu-id="9bf97-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf97-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf97-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bf97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9bf97-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9bf97-119">Request headers</span></span>
|<span data-ttu-id="9bf97-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bf97-120">Header</span></span>|<span data-ttu-id="9bf97-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9bf97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bf97-122">Authorization</span></span>|<span data-ttu-id="9bf97-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bf97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf97-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9bf97-124">Accept</span></span>|<span data-ttu-id="9bf97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf97-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bf97-126">Request body</span></span>
<span data-ttu-id="9bf97-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bf97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bf97-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bf97-128">Response</span></span>
<span data-ttu-id="9bf97-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9bf97-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf97-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9bf97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf97-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bf97-131">Request</span></span>
<span data-ttu-id="9bf97-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bf97-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="9bf97-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bf97-133">Response</span></span>
<span data-ttu-id="9bf97-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bf97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




