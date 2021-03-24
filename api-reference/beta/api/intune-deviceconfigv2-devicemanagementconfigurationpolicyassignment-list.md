---
title: Список deviceManagementConfigurationPolicyAssignments
description: Список свойств и связей объектов deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdb3eea81cca8aed016f57277bc446935e0803a4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147065"
---
# <a name="list-devicemanagementconfigurationpolicyassignments"></a><span data-ttu-id="7aa68-103">Список deviceManagementConfigurationPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="7aa68-103">List deviceManagementConfigurationPolicyAssignments</span></span>

<span data-ttu-id="7aa68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7aa68-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7aa68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7aa68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aa68-107">Список свойств и связей [объектов deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7aa68-107">List properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aa68-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7aa68-108">Prerequisites</span></span>
<span data-ttu-id="7aa68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa68-111">Permission type</span></span>|<span data-ttu-id="7aa68-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aa68-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aa68-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aa68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7aa68-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa68-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7aa68-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aa68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aa68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa68-116">Not supported.</span></span>|
|<span data-ttu-id="7aa68-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7aa68-117">Application</span></span>|<span data-ttu-id="7aa68-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa68-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7aa68-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7aa68-120">Request headers</span></span>
|<span data-ttu-id="7aa68-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aa68-121">Header</span></span>|<span data-ttu-id="7aa68-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aa68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa68-123">Authorization</span></span>|<span data-ttu-id="7aa68-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aa68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aa68-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7aa68-125">Accept</span></span>|<span data-ttu-id="7aa68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aa68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7aa68-127">Request body</span></span>
<span data-ttu-id="7aa68-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7aa68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aa68-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aa68-129">Response</span></span>
<span data-ttu-id="7aa68-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7aa68-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa68-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7aa68-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aa68-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aa68-132">Request</span></span>
<span data-ttu-id="7aa68-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aa68-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="7aa68-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aa68-134">Response</span></span>
<span data-ttu-id="7aa68-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7aa68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




