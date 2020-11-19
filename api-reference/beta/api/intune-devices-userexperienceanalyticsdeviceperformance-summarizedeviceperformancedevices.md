---
title: Функция Суммаризедевицеперформанцедевицес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3b88a91ce23f151b0048179a4190babb6cb8817
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234330"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="4f6bd-103">Функция Суммаризедевицеперформанцедевицес</span><span class="sxs-lookup"><span data-stu-id="4f6bd-103">summarizeDevicePerformanceDevices function</span></span>

<span data-ttu-id="4f6bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f6bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f6bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f6bd-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f6bd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f6bd-108">Prerequisites</span></span>
<span data-ttu-id="4f6bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6bd-111">Permission type</span></span>|<span data-ttu-id="4f6bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f6bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f6bd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f6bd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4f6bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f6bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-116">Not supported.</span></span>|
|<span data-ttu-id="4f6bd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f6bd-117">Application</span></span>|<span data-ttu-id="4f6bd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f6bd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f6bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="4f6bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f6bd-120">Request headers</span></span>
|<span data-ttu-id="4f6bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f6bd-121">Header</span></span>|<span data-ttu-id="4f6bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f6bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f6bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f6bd-123">Authorization</span></span>|<span data-ttu-id="4f6bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f6bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f6bd-125">Accept</span></span>|<span data-ttu-id="4f6bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f6bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f6bd-127">Request body</span></span>
<span data-ttu-id="4f6bd-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4f6bd-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4f6bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f6bd-130">Property</span></span>|<span data-ttu-id="4f6bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6bd-131">Type</span></span>|<span data-ttu-id="4f6bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f6bd-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="4f6bd-133">summarizeBy</span></span>|[<span data-ttu-id="4f6bd-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="4f6bd-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="4f6bd-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f6bd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f6bd-136">Response</span></span>
<span data-ttu-id="4f6bd-137">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f6bd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4f6bd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f6bd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bd-139">Request</span></span>
<span data-ttu-id="4f6bd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4f6bd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bd-141">Response</span></span>
<span data-ttu-id="4f6bd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f6bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




