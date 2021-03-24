---
title: Get deviceManagementConfigurationPolicyAssignment
description: Чтение свойств и связей объекта deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e661013e9d864e99474efdfc603f3760e9fb380
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132200"
---
# <a name="get-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="09a40-103">Get deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="09a40-103">Get deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="09a40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09a40-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09a40-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a40-107">Чтение свойств и связей [объекта deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09a40-107">Read properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09a40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09a40-108">Prerequisites</span></span>
<span data-ttu-id="09a40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09a40-111">Permission type</span></span>|<span data-ttu-id="09a40-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09a40-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09a40-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09a40-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a40-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09a40-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09a40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09a40-116">Not supported.</span></span>|
|<span data-ttu-id="09a40-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="09a40-117">Application</span></span>|<span data-ttu-id="09a40-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a40-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09a40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09a40-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09a40-120">Optional query parameters</span></span>
<span data-ttu-id="09a40-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="09a40-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09a40-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09a40-122">Request headers</span></span>
|<span data-ttu-id="09a40-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09a40-123">Header</span></span>|<span data-ttu-id="09a40-124">Значение</span><span class="sxs-lookup"><span data-stu-id="09a40-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09a40-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="09a40-125">Authorization</span></span>|<span data-ttu-id="09a40-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09a40-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09a40-127">Accept</span><span class="sxs-lookup"><span data-stu-id="09a40-127">Accept</span></span>|<span data-ttu-id="09a40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="09a40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a40-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09a40-129">Request body</span></span>
<span data-ttu-id="09a40-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09a40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09a40-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="09a40-131">Response</span></span>
<span data-ttu-id="09a40-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="09a40-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a40-133">Пример</span><span class="sxs-lookup"><span data-stu-id="09a40-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="09a40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="09a40-134">Request</span></span>
<span data-ttu-id="09a40-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09a40-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="09a40-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="09a40-136">Response</span></span>
<span data-ttu-id="09a40-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09a40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
    "id": "1f069921-9921-1f06-2199-061f2199061f",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    }
  }
}
```




