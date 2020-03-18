---
title: Функция Суммаризедевицерегрессионперформанце
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50413f9d1a38d780d91b55a2c7908487fb70c32a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813791"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="58917-103">Функция Суммаризедевицерегрессионперформанце</span><span class="sxs-lookup"><span data-stu-id="58917-103">summarizeDeviceRegressionPerformance function</span></span>

> <span data-ttu-id="58917-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58917-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58917-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58917-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58917-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58917-107">Prerequisites</span></span>
<span data-ttu-id="58917-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58917-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58917-110">Permission type</span></span>|<span data-ttu-id="58917-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58917-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58917-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58917-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58917-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58917-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="58917-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58917-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58917-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58917-115">Not supported.</span></span>|
|<span data-ttu-id="58917-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="58917-116">Application</span></span>|<span data-ttu-id="58917-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58917-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58917-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58917-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="58917-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58917-119">Request headers</span></span>
|<span data-ttu-id="58917-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58917-120">Header</span></span>|<span data-ttu-id="58917-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58917-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58917-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58917-122">Authorization</span></span>|<span data-ttu-id="58917-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58917-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58917-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58917-124">Accept</span></span>|<span data-ttu-id="58917-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58917-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58917-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58917-126">Request body</span></span>
<span data-ttu-id="58917-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="58917-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="58917-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="58917-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="58917-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58917-129">Property</span></span>|<span data-ttu-id="58917-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58917-130">Type</span></span>|<span data-ttu-id="58917-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58917-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58917-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="58917-132">summarizeBy</span></span>|[<span data-ttu-id="58917-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="58917-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="58917-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="58917-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58917-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="58917-135">Response</span></span>
<span data-ttu-id="58917-136">В случае успеха эта функция возвращает код `200 OK` отклика и объект [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58917-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58917-137">Пример</span><span class="sxs-lookup"><span data-stu-id="58917-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="58917-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="58917-138">Request</span></span>
<span data-ttu-id="58917-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58917-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="58917-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58917-140">Response</span></span>
<span data-ttu-id="58917-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58917-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




