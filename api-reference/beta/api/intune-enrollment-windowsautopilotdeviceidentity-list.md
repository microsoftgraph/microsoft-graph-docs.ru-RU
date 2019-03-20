---
title: Список Виндовсаутопилотдевицеидентитиес
description: Список свойств и связей объектов windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1520238c53db908b7c5801b679275216b97ef47
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572252"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="b59f1-103">Список Виндовсаутопилотдевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="b59f1-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="b59f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b59f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b59f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b59f1-106">Список свойств и связей объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="b59f1-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b59f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b59f1-107">Prerequisites</span></span>
<span data-ttu-id="b59f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b59f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b59f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b59f1-110">Permission type</span></span>|<span data-ttu-id="b59f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b59f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b59f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b59f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b59f1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b59f1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b59f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b59f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b59f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59f1-115">Not supported.</span></span>|
|<span data-ttu-id="b59f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b59f1-116">Application</span></span>|<span data-ttu-id="b59f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b59f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b59f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="b59f1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b59f1-119">Request headers</span></span>
|<span data-ttu-id="b59f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b59f1-120">Header</span></span>|<span data-ttu-id="b59f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b59f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b59f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b59f1-122">Authorization</span></span>|<span data-ttu-id="b59f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b59f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b59f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b59f1-124">Accept</span></span>|<span data-ttu-id="b59f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b59f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b59f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b59f1-126">Request body</span></span>
<span data-ttu-id="b59f1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b59f1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59f1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b59f1-128">Response</span></span>
<span data-ttu-id="b59f1-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b59f1-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b59f1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b59f1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b59f1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59f1-131">Request</span></span>
<span data-ttu-id="b59f1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b59f1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="b59f1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59f1-133">Response</span></span>
<span data-ttu-id="b59f1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b59f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1163

{
  "value": [
    {
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
  ]
}
```




