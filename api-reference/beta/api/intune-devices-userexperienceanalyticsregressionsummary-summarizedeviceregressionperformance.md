---
title: summarizeDeviceRegressionPerformance function
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce1c44aa32b7e8ad4885d8766f16eb97f35204b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135987"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="a3dc8-103">summarizeDeviceRegressionPerformance function</span><span class="sxs-lookup"><span data-stu-id="a3dc8-103">summarizeDeviceRegressionPerformance function</span></span>

<span data-ttu-id="a3dc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3dc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3dc8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3dc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3dc8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3dc8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3dc8-108">Prerequisites</span></span>
<span data-ttu-id="a3dc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3dc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3dc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3dc8-111">Permission type</span></span>|<span data-ttu-id="a3dc8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3dc8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3dc8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3dc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3dc8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3dc8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3dc8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3dc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3dc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-116">Not supported.</span></span>|
|<span data-ttu-id="a3dc8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3dc8-117">Application</span></span>|<span data-ttu-id="a3dc8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3dc8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3dc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3dc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="a3dc8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3dc8-120">Request headers</span></span>
|<span data-ttu-id="a3dc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3dc8-121">Header</span></span>|<span data-ttu-id="a3dc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3dc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3dc8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3dc8-123">Authorization</span></span>|<span data-ttu-id="a3dc8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3dc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3dc8-125">Accept</span></span>|<span data-ttu-id="a3dc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3dc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3dc8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3dc8-127">Request body</span></span>
<span data-ttu-id="a3dc8-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a3dc8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a3dc8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3dc8-130">Property</span></span>|<span data-ttu-id="a3dc8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3dc8-131">Type</span></span>|<span data-ttu-id="a3dc8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3dc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3dc8-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="a3dc8-133">summarizeBy</span></span>|[<span data-ttu-id="a3dc8-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="a3dc8-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="a3dc8-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a3dc8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3dc8-136">Response</span></span>
<span data-ttu-id="a3dc8-137">В случае успешной данной функции возвращается код отклика и `200 OK` [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3dc8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a3dc8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3dc8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3dc8-139">Request</span></span>
<span data-ttu-id="a3dc8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a3dc8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3dc8-141">Response</span></span>
<span data-ttu-id="a3dc8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3dc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 154

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
    "id": "41683327-3327-4168-2733-684127336841"
  }
}
```




