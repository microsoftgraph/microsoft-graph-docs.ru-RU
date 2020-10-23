---
title: Список Виндовсаутопилотдевицеидентитиес
description: Список свойств и связей объектов windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18d8c681dcd5c9bbc3dc44feeeeb98169dd06119
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696645"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="e5ed1-103">Список Виндовсаутопилотдевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="e5ed1-103">List windowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="e5ed1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5ed1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5ed1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5ed1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ed1-107">Список свойств и связей объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="e5ed1-107">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5ed1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5ed1-108">Prerequisites</span></span>
<span data-ttu-id="e5ed1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5ed1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ed1-111">Permission type</span></span>|<span data-ttu-id="e5ed1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5ed1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5ed1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5ed1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5ed1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5ed1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e5ed1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5ed1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5ed1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-116">Not supported.</span></span>|
|<span data-ttu-id="e5ed1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5ed1-117">Application</span></span>|<span data-ttu-id="e5ed1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5ed1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5ed1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5ed1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="e5ed1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5ed1-120">Request headers</span></span>
|<span data-ttu-id="e5ed1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5ed1-121">Header</span></span>|<span data-ttu-id="e5ed1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5ed1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5ed1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5ed1-123">Authorization</span></span>|<span data-ttu-id="e5ed1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5ed1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5ed1-125">Accept</span></span>|<span data-ttu-id="e5ed1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5ed1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5ed1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5ed1-127">Request body</span></span>
<span data-ttu-id="e5ed1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ed1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5ed1-129">Response</span></span>
<span data-ttu-id="e5ed1-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5ed1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ed1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5ed1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5ed1-132">Request</span></span>
<span data-ttu-id="e5ed1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="e5ed1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ed1-134">Response</span></span>
<span data-ttu-id="e5ed1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5ed1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "deploymentProfileAssignmentStatus": "assignedInSync",
      "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
      "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
      "orderIdentifier": "Order Identifier value",
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





