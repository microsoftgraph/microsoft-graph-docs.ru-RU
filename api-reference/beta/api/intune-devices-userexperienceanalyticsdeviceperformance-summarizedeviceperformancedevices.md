---
title: Функция Суммаризедевицеперформанцедевицес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1a0abea2af97b68a60f2fe0abc52ce3431adf92
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529216"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="31807-103">Функция Суммаризедевицеперформанцедевицес</span><span class="sxs-lookup"><span data-stu-id="31807-103">summarizeDevicePerformanceDevices function</span></span>

> <span data-ttu-id="31807-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31807-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31807-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31807-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31807-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="31807-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31807-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31807-107">Prerequisites</span></span>
<span data-ttu-id="31807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31807-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31807-110">Permission type</span></span>|<span data-ttu-id="31807-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31807-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31807-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31807-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31807-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="31807-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="31807-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31807-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31807-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31807-115">Not supported.</span></span>|
|<span data-ttu-id="31807-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="31807-116">Application</span></span>|<span data-ttu-id="31807-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="31807-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31807-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31807-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="31807-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31807-119">Request headers</span></span>
|<span data-ttu-id="31807-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31807-120">Header</span></span>|<span data-ttu-id="31807-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31807-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31807-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31807-122">Authorization</span></span>|<span data-ttu-id="31807-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31807-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31807-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31807-124">Accept</span></span>|<span data-ttu-id="31807-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31807-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31807-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31807-126">Request body</span></span>
<span data-ttu-id="31807-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="31807-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="31807-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="31807-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="31807-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="31807-129">Property</span></span>|<span data-ttu-id="31807-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31807-130">Type</span></span>|<span data-ttu-id="31807-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31807-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31807-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="31807-132">summarizeBy</span></span>|[<span data-ttu-id="31807-133">усерекспериенцеаналитикссуммаризедби</span><span class="sxs-lookup"><span data-stu-id="31807-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="31807-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="31807-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="31807-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="31807-135">Response</span></span>
<span data-ttu-id="31807-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31807-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31807-137">Пример</span><span class="sxs-lookup"><span data-stu-id="31807-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="31807-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="31807-138">Request</span></span>
<span data-ttu-id="31807-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31807-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="31807-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="31807-140">Response</span></span>
<span data-ttu-id="31807-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31807-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

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
      "deviceCount": 11
    }
  ]
}
```






