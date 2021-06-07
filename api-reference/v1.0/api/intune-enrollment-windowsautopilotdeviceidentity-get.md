---
title: Get windowsAutopilotDeviceIdentity
description: Чтение свойств и связей объекта windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8039791e1371d50cf38c69dd6026bfeffc7463e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753383"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="cf5c0-103">Get windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cf5c0-103">Get windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="cf5c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf5c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf5c0-106">Чтение свойств и связей объекта [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-106">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf5c0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf5c0-107">Prerequisites</span></span>
<span data-ttu-id="cf5c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5c0-110">Permission type</span></span>|<span data-ttu-id="cf5c0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf5c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf5c0-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5c0-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf5c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf5c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-115">Not supported.</span></span>|
|<span data-ttu-id="cf5c0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf5c0-116">Application</span></span>|<span data-ttu-id="cf5c0-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5c0-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf5c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf5c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf5c0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf5c0-119">Optional query parameters</span></span>
<span data-ttu-id="cf5c0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf5c0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf5c0-121">Request headers</span></span>
|<span data-ttu-id="cf5c0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf5c0-122">Header</span></span>|<span data-ttu-id="cf5c0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cf5c0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf5c0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf5c0-124">Authorization</span></span>|<span data-ttu-id="cf5c0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf5c0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cf5c0-126">Accept</span></span>|<span data-ttu-id="cf5c0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf5c0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf5c0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf5c0-128">Request body</span></span>
<span data-ttu-id="cf5c0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf5c0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5c0-130">Response</span></span>
<span data-ttu-id="cf5c0-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5c0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cf5c0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf5c0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf5c0-133">Request</span></span>
<span data-ttu-id="cf5c0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="cf5c0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5c0-135">Response</span></span>
<span data-ttu-id="cf5c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
    "groupTag": "Group Tag value",
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
    "managedDeviceId": "Managed Device Id value",
    "displayName": "Display Name value"
  }
}
```




