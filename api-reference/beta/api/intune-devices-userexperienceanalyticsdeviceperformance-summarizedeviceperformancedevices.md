---
title: Функция Суммаризедевицеперформанцедевицес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c66c72a27296c3b28460874899e7a0b78bde760
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468399"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="978aa-103">Функция Суммаризедевицеперформанцедевицес</span><span class="sxs-lookup"><span data-stu-id="978aa-103">summarizeDevicePerformanceDevices function</span></span>

<span data-ttu-id="978aa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="978aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="978aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="978aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="978aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978aa-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="978aa-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="978aa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="978aa-108">Prerequisites</span></span>
<span data-ttu-id="978aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="978aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="978aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="978aa-111">Permission type</span></span>|<span data-ttu-id="978aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="978aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="978aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="978aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="978aa-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="978aa-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="978aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="978aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="978aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978aa-116">Not supported.</span></span>|
|<span data-ttu-id="978aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="978aa-117">Application</span></span>|<span data-ttu-id="978aa-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="978aa-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="978aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="978aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="978aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="978aa-120">Request headers</span></span>
|<span data-ttu-id="978aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="978aa-121">Header</span></span>|<span data-ttu-id="978aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="978aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="978aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="978aa-123">Authorization</span></span>|<span data-ttu-id="978aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="978aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="978aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="978aa-125">Accept</span></span>|<span data-ttu-id="978aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="978aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="978aa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="978aa-127">Request body</span></span>
<span data-ttu-id="978aa-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="978aa-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="978aa-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="978aa-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="978aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="978aa-130">Property</span></span>|<span data-ttu-id="978aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="978aa-131">Type</span></span>|<span data-ttu-id="978aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="978aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978aa-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="978aa-133">summarizeBy</span></span>|[<span data-ttu-id="978aa-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="978aa-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="978aa-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="978aa-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="978aa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="978aa-136">Response</span></span>
<span data-ttu-id="978aa-137">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="978aa-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="978aa-138">Пример</span><span class="sxs-lookup"><span data-stu-id="978aa-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="978aa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="978aa-139">Request</span></span>
<span data-ttu-id="978aa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="978aa-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="978aa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="978aa-141">Response</span></span>
<span data-ttu-id="978aa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="978aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9
    }
  ]
}
```





