---
title: Список Усерекспериенцеаналитиксдевицестартуппроцессперформанцес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ed9001fbbc7be6956e048004b1e38a05ef1ea79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468259"
---
# <a name="list-userexperienceanalyticsdevicestartupprocessperformances"></a><span data-ttu-id="09e6e-103">Список Усерекспериенцеаналитиксдевицестартуппроцессперформанцес</span><span class="sxs-lookup"><span data-stu-id="09e6e-103">List userExperienceAnalyticsDeviceStartupProcessPerformances</span></span>

<span data-ttu-id="09e6e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09e6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09e6e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09e6e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09e6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09e6e-107">Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="09e6e-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09e6e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09e6e-108">Prerequisites</span></span>
<span data-ttu-id="09e6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e6e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09e6e-111">Permission type</span></span>|<span data-ttu-id="09e6e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09e6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09e6e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09e6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09e6e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e6e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="09e6e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09e6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09e6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e6e-116">Not supported.</span></span>|
|<span data-ttu-id="09e6e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09e6e-117">Application</span></span>|<span data-ttu-id="09e6e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e6e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09e6e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09e6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="09e6e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09e6e-120">Request headers</span></span>
|<span data-ttu-id="09e6e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09e6e-121">Header</span></span>|<span data-ttu-id="09e6e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09e6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09e6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e6e-123">Authorization</span></span>|<span data-ttu-id="09e6e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09e6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09e6e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09e6e-125">Accept</span></span>|<span data-ttu-id="09e6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09e6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09e6e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09e6e-127">Request body</span></span>
<span data-ttu-id="09e6e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09e6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09e6e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="09e6e-129">Response</span></span>
<span data-ttu-id="09e6e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09e6e-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e6e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="09e6e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="09e6e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="09e6e-132">Request</span></span>
<span data-ttu-id="09e6e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09e6e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

### <a name="response"></a><span data-ttu-id="09e6e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="09e6e-134">Response</span></span>
<span data-ttu-id="09e6e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09e6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
      "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
      "processName": "Process Name value",
      "productName": "Product Name value",
      "publisher": "Publisher value",
      "deviceCount": 11,
      "medianImpactInMs": 0,
      "totalImpactInMs": 15
    }
  ]
}
```





