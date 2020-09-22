---
title: Список Усерекспериенцеаналитиксдевицестартуппроцессес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицестартуппроцесс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fed1a96c56ff057c87468de6f6f9c2711c70eb55
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082527"
---
# <a name="list-userexperienceanalyticsdevicestartupprocesses"></a><span data-ttu-id="cc322-103">Список Усерекспериенцеаналитиксдевицестартуппроцессес</span><span class="sxs-lookup"><span data-stu-id="cc322-103">List userExperienceAnalyticsDeviceStartupProcesses</span></span>

<span data-ttu-id="cc322-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc322-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc322-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc322-107">Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="cc322-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc322-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc322-108">Prerequisites</span></span>
<span data-ttu-id="cc322-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc322-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc322-111">Permission type</span></span>|<span data-ttu-id="cc322-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc322-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc322-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc322-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc322-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cc322-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc322-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc322-116">Not supported.</span></span>|
|<span data-ttu-id="cc322-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc322-117">Application</span></span>|<span data-ttu-id="cc322-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc322-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc322-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="cc322-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc322-120">Request headers</span></span>
|<span data-ttu-id="cc322-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc322-121">Header</span></span>|<span data-ttu-id="cc322-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc322-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc322-123">Authorization</span></span>|<span data-ttu-id="cc322-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc322-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc322-125">Accept</span></span>|<span data-ttu-id="cc322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc322-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc322-127">Request body</span></span>
<span data-ttu-id="cc322-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc322-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc322-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc322-129">Response</span></span>
<span data-ttu-id="cc322-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc322-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc322-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cc322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc322-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc322-132">Request</span></span>
<span data-ttu-id="cc322-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc322-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

### <a name="response"></a><span data-ttu-id="cc322-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc322-134">Response</span></span>
<span data-ttu-id="cc322-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc322-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 386

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
      "id": "03b451e6-51e6-03b4-e651-b403e651b403",
      "managedDeviceId": "Managed Device Id value",
      "processName": "Process Name value",
      "productName": "Product Name value",
      "publisher": "Publisher value",
      "startupImpactInMs": 1
    }
  ]
}
```






