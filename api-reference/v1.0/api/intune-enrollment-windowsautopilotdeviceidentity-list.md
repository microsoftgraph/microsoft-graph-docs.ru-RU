---
title: Список windowsAutopilotDeviceIdentities
description: Список свойств и связей объектов windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76433afb73b62b80df51e6c4962256d965b3babd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753382"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="6b7ad-103">Список windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="6b7ad-103">List windowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="6b7ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b7ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b7ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b7ad-106">Список свойств и связей объектов [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="6b7ad-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b7ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b7ad-107">Prerequisites</span></span>
<span data-ttu-id="6b7ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b7ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b7ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b7ad-110">Permission type</span></span>|<span data-ttu-id="6b7ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b7ad-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b7ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b7ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b7ad-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7ad-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6b7ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b7ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b7ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-115">Not supported.</span></span>|
|<span data-ttu-id="6b7ad-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b7ad-116">Application</span></span>|<span data-ttu-id="6b7ad-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7ad-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b7ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b7ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6b7ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6b7ad-119">Request headers</span></span>
|<span data-ttu-id="6b7ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b7ad-120">Header</span></span>|<span data-ttu-id="6b7ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b7ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b7ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b7ad-122">Authorization</span></span>|<span data-ttu-id="6b7ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b7ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b7ad-124">Accept</span></span>|<span data-ttu-id="6b7ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b7ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b7ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b7ad-126">Request body</span></span>
<span data-ttu-id="6b7ad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b7ad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b7ad-128">Response</span></span>
<span data-ttu-id="6b7ad-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b7ad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6b7ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b7ad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b7ad-131">Request</span></span>
<span data-ttu-id="6b7ad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="6b7ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b7ad-133">Response</span></span>
<span data-ttu-id="6b7ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b7ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "value": [
    {
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
  ]
}
```




