---
title: Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Чтение свойств и связей объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 435a03b0b0fdd7b5a2580b19a7c8c6d549007437
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473926"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="a1503-103">Получение Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="a1503-103">Get windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="a1503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1503-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1503-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1503-107">Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a1503-107">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1503-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1503-108">Prerequisites</span></span>
<span data-ttu-id="a1503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1503-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1503-111">Permission type</span></span>|<span data-ttu-id="a1503-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1503-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1503-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1503-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1503-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1503-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1503-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1503-116">Not supported.</span></span>|
|<span data-ttu-id="a1503-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1503-117">Application</span></span>|<span data-ttu-id="a1503-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1503-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1503-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1503-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1503-120">Optional query parameters</span></span>
<span data-ttu-id="a1503-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1503-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1503-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1503-122">Request headers</span></span>
|<span data-ttu-id="a1503-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1503-123">Header</span></span>|<span data-ttu-id="a1503-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a1503-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1503-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1503-125">Authorization</span></span>|<span data-ttu-id="a1503-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1503-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1503-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a1503-127">Accept</span></span>|<span data-ttu-id="a1503-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1503-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1503-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1503-129">Request body</span></span>
<span data-ttu-id="a1503-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1503-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1503-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1503-131">Response</span></span>
<span data-ttu-id="a1503-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1503-132">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1503-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a1503-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1503-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1503-134">Request</span></span>
<span data-ttu-id="a1503-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1503-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

### <a name="response"></a><span data-ttu-id="a1503-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1503-136">Response</span></span>
<span data-ttu-id="a1503-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1503-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
    "id": "e3c01841-1841-e3c0-4118-c0e34118c0e3",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "deploymentStatus": "success",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "policyVersion": "Policy Version value"
  }
}
```



