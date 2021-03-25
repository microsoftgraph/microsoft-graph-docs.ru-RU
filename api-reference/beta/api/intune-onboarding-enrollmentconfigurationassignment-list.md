---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 678af5356670e6699b4c42ed9ead1ed4b6e1fd85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156886"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="ddc49-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ddc49-103">List enrollmentConfigurationAssignments</span></span>

<span data-ttu-id="ddc49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddc49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddc49-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddc49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddc49-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddc49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddc49-107">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddc49-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddc49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddc49-108">Prerequisites</span></span>
<span data-ttu-id="ddc49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddc49-111">Permission type</span></span>|<span data-ttu-id="ddc49-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddc49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddc49-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddc49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddc49-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddc49-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ddc49-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddc49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddc49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddc49-116">Not supported.</span></span>|
|<span data-ttu-id="ddc49-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ddc49-117">Application</span></span>|<span data-ttu-id="ddc49-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddc49-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddc49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddc49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ddc49-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddc49-120">Request headers</span></span>
|<span data-ttu-id="ddc49-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddc49-121">Header</span></span>|<span data-ttu-id="ddc49-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ddc49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddc49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddc49-123">Authorization</span></span>|<span data-ttu-id="ddc49-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddc49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddc49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddc49-125">Accept</span></span>|<span data-ttu-id="ddc49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddc49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddc49-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddc49-127">Request body</span></span>
<span data-ttu-id="ddc49-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddc49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc49-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddc49-129">Response</span></span>
<span data-ttu-id="ddc49-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddc49-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddc49-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ddc49-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddc49-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddc49-132">Request</span></span>
<span data-ttu-id="ddc49-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddc49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="ddc49-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddc49-134">Response</span></span>
<span data-ttu-id="ddc49-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddc49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




