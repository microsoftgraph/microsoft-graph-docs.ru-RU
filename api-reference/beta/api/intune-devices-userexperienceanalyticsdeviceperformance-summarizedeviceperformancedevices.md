---
title: Функция Суммаризедевицеперформанцедевицес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10752b98e4d27c9f300c16c7b2e4a597048d7fc4
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791465"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="a327d-103">Функция Суммаризедевицеперформанцедевицес</span><span class="sxs-lookup"><span data-stu-id="a327d-103">summarizeDevicePerformanceDevices function</span></span>

<span data-ttu-id="a327d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a327d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a327d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a327d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a327d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a327d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a327d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a327d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a327d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a327d-108">Prerequisites</span></span>
<span data-ttu-id="a327d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a327d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a327d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a327d-111">Permission type</span></span>|<span data-ttu-id="a327d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a327d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a327d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a327d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a327d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a327d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a327d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a327d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a327d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a327d-116">Not supported.</span></span>|
|<span data-ttu-id="a327d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a327d-117">Application</span></span>|<span data-ttu-id="a327d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a327d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a327d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a327d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="a327d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a327d-120">Request headers</span></span>
|<span data-ttu-id="a327d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a327d-121">Header</span></span>|<span data-ttu-id="a327d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a327d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a327d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a327d-123">Authorization</span></span>|<span data-ttu-id="a327d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a327d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a327d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a327d-125">Accept</span></span>|<span data-ttu-id="a327d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a327d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a327d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a327d-127">Request body</span></span>
<span data-ttu-id="a327d-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a327d-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a327d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a327d-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a327d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a327d-130">Property</span></span>|<span data-ttu-id="a327d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a327d-131">Type</span></span>|<span data-ttu-id="a327d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a327d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a327d-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="a327d-133">summarizeBy</span></span>|[<span data-ttu-id="a327d-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="a327d-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="a327d-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a327d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a327d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a327d-136">Response</span></span>
<span data-ttu-id="a327d-137">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a327d-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a327d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a327d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a327d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a327d-139">Request</span></span>
<span data-ttu-id="a327d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a327d-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a327d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a327d-141">Response</span></span>
<span data-ttu-id="a327d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a327d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

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
      "responsiveDesktopTimeInMs": 9,
      "blueScreenCount": 15,
      "restartCount": 12,
      "averageBlueScreens": 6.0,
      "averageRestarts": 5.0
    }
  ]
}
```



