---
title: Функция Суммаризедевицерегрессионперформанце
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a38362abb310d536b04cb5c4c58b0f93b1ed8ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468063"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="bea5c-103">Функция Суммаризедевицерегрессионперформанце</span><span class="sxs-lookup"><span data-stu-id="bea5c-103">summarizeDeviceRegressionPerformance function</span></span>

<span data-ttu-id="bea5c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bea5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bea5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bea5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bea5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea5c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bea5c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bea5c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bea5c-108">Prerequisites</span></span>
<span data-ttu-id="bea5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bea5c-111">Permission type</span></span>|<span data-ttu-id="bea5c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bea5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bea5c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bea5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bea5c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bea5c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bea5c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bea5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bea5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea5c-116">Not supported.</span></span>|
|<span data-ttu-id="bea5c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bea5c-117">Application</span></span>|<span data-ttu-id="bea5c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bea5c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bea5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bea5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="bea5c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bea5c-120">Request headers</span></span>
|<span data-ttu-id="bea5c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bea5c-121">Header</span></span>|<span data-ttu-id="bea5c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bea5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bea5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea5c-123">Authorization</span></span>|<span data-ttu-id="bea5c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bea5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bea5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bea5c-125">Accept</span></span>|<span data-ttu-id="bea5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bea5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea5c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bea5c-127">Request body</span></span>
<span data-ttu-id="bea5c-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="bea5c-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bea5c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="bea5c-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bea5c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bea5c-130">Property</span></span>|<span data-ttu-id="bea5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bea5c-131">Type</span></span>|<span data-ttu-id="bea5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bea5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea5c-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="bea5c-133">summarizeBy</span></span>|[<span data-ttu-id="bea5c-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="bea5c-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="bea5c-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bea5c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bea5c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bea5c-136">Response</span></span>
<span data-ttu-id="bea5c-137">В случае успеха эта функция возвращает код `200 OK` отклика и объект [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bea5c-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea5c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bea5c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bea5c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bea5c-139">Request</span></span>
<span data-ttu-id="bea5c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bea5c-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bea5c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea5c-141">Response</span></span>
<span data-ttu-id="bea5c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bea5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





