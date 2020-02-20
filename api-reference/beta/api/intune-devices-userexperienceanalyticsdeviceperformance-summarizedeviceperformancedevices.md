---
title: Функция Суммаризедевицеперформанцедевицес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf3bfd84f2f0d206553d955c74adfe05f7add6a5
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162052"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="7c323-103">Функция Суммаризедевицеперформанцедевицес</span><span class="sxs-lookup"><span data-stu-id="7c323-103">summarizeDevicePerformanceDevices function</span></span>

> <span data-ttu-id="7c323-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c323-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c323-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c323-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c323-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c323-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c323-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c323-107">Prerequisites</span></span>
<span data-ttu-id="7c323-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c323-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c323-110">Permission type</span></span>|<span data-ttu-id="7c323-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c323-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c323-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c323-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c323-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c323-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7c323-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c323-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c323-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c323-115">Not supported.</span></span>|
|<span data-ttu-id="7c323-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c323-116">Application</span></span>|<span data-ttu-id="7c323-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c323-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c323-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c323-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="7c323-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c323-119">Request headers</span></span>
|<span data-ttu-id="7c323-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c323-120">Header</span></span>|<span data-ttu-id="7c323-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c323-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c323-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c323-122">Authorization</span></span>|<span data-ttu-id="7c323-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c323-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c323-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c323-124">Accept</span></span>|<span data-ttu-id="7c323-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c323-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c323-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c323-126">Request body</span></span>
<span data-ttu-id="7c323-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7c323-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7c323-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="7c323-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7c323-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c323-129">Property</span></span>|<span data-ttu-id="7c323-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c323-130">Type</span></span>|<span data-ttu-id="7c323-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c323-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c323-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="7c323-132">summarizeBy</span></span>|[<span data-ttu-id="7c323-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="7c323-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="7c323-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c323-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c323-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c323-135">Response</span></span>
<span data-ttu-id="7c323-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c323-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c323-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7c323-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c323-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c323-138">Request</span></span>
<span data-ttu-id="7c323-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c323-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7c323-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c323-140">Response</span></span>
<span data-ttu-id="7c323-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c323-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





