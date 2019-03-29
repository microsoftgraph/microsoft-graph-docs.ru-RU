---
title: Получение windowsAutopilotDeviceIdentity
description: Чтение свойств и связей объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db567c3d79e6df3a4f03603fa7506c3c451d4476
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959812"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="dba2b-103">Получение windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="dba2b-103">Get windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="dba2b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba2b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dba2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba2b-106">Чтение свойств и связей объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="dba2b-106">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dba2b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dba2b-107">Prerequisites</span></span>
<span data-ttu-id="dba2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dba2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dba2b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dba2b-110">Permission type</span></span>|<span data-ttu-id="dba2b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dba2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dba2b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dba2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dba2b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dba2b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dba2b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dba2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dba2b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba2b-115">Not supported.</span></span>|
|<span data-ttu-id="dba2b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dba2b-116">Application</span></span>|<span data-ttu-id="dba2b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba2b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dba2b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dba2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dba2b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dba2b-119">Optional query parameters</span></span>
<span data-ttu-id="dba2b-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dba2b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dba2b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dba2b-121">Request headers</span></span>
|<span data-ttu-id="dba2b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dba2b-122">Header</span></span>|<span data-ttu-id="dba2b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dba2b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dba2b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dba2b-124">Authorization</span></span>|<span data-ttu-id="dba2b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dba2b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dba2b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dba2b-126">Accept</span></span>|<span data-ttu-id="dba2b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dba2b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dba2b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dba2b-128">Request body</span></span>
<span data-ttu-id="dba2b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dba2b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dba2b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dba2b-130">Response</span></span>
<span data-ttu-id="dba2b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dba2b-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dba2b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dba2b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dba2b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dba2b-133">Request</span></span>
<span data-ttu-id="dba2b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dba2b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="dba2b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dba2b-135">Response</span></span>
<span data-ttu-id="dba2b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dba2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1109

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
    "deploymentProfileAssignmentStatus": "assignedInSync",
    "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
    "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
    "orderIdentifier": "Order Identifier value",
    "purchaseOrderIdentifier": "Purchase Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "enrollmentState": "enrolled",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "addressableUserName": "Addressable User Name value",
    "userPrincipalName": "User Principal Name value",
    "resourceName": "Resource Name value",
    "skuNumber": "Sku Number value",
    "systemFamily": "System Family value",
    "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
    "managedDeviceId": "Managed Device Id value"
  }
}
```




