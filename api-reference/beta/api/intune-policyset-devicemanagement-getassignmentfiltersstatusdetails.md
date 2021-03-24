---
title: действие getAssignmentFiltersStatusDetails
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2538cc410dbe3b80ea1b2e26c5fe3c4c9bedafca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148675"
---
# <a name="getassignmentfiltersstatusdetails-action"></a><span data-ttu-id="36f0c-103">действие getAssignmentFiltersStatusDetails</span><span class="sxs-lookup"><span data-stu-id="36f0c-103">getAssignmentFiltersStatusDetails action</span></span>

<span data-ttu-id="36f0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36f0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36f0c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36f0c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36f0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36f0c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36f0c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36f0c-108">Prerequisites</span></span>
<span data-ttu-id="36f0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36f0c-111">Permission type</span></span>|<span data-ttu-id="36f0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36f0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36f0c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36f0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36f0c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f0c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36f0c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36f0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36f0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f0c-116">Not supported.</span></span>|
|<span data-ttu-id="36f0c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="36f0c-117">Application</span></span>|<span data-ttu-id="36f0c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f0c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36f0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36f0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/getAssignmentFiltersStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="36f0c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36f0c-120">Request headers</span></span>
|<span data-ttu-id="36f0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36f0c-121">Header</span></span>|<span data-ttu-id="36f0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36f0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36f0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f0c-123">Authorization</span></span>|<span data-ttu-id="36f0c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36f0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36f0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36f0c-125">Accept</span></span>|<span data-ttu-id="36f0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36f0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36f0c-127">Request body</span></span>
<span data-ttu-id="36f0c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36f0c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="36f0c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="36f0c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="36f0c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36f0c-130">Property</span></span>|<span data-ttu-id="36f0c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36f0c-131">Type</span></span>|<span data-ttu-id="36f0c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36f0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36f0c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="36f0c-133">managedDeviceId</span></span>|<span data-ttu-id="36f0c-134">String</span><span class="sxs-lookup"><span data-stu-id="36f0c-134">String</span></span>|<span data-ttu-id="36f0c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-135">Not yet documented</span></span>|
|<span data-ttu-id="36f0c-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="36f0c-136">payloadId</span></span>|<span data-ttu-id="36f0c-137">String</span><span class="sxs-lookup"><span data-stu-id="36f0c-137">String</span></span>|<span data-ttu-id="36f0c-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-138">Not yet documented</span></span>|
|<span data-ttu-id="36f0c-139">userId</span><span class="sxs-lookup"><span data-stu-id="36f0c-139">userId</span></span>|<span data-ttu-id="36f0c-140">String</span><span class="sxs-lookup"><span data-stu-id="36f0c-140">String</span></span>|<span data-ttu-id="36f0c-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-141">Not yet documented</span></span>|
|<span data-ttu-id="36f0c-142">assignmentFilterIds</span><span class="sxs-lookup"><span data-stu-id="36f0c-142">assignmentFilterIds</span></span>|<span data-ttu-id="36f0c-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36f0c-143">String collection</span></span>|<span data-ttu-id="36f0c-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36f0c-144">Not yet documented</span></span>|
|<span data-ttu-id="36f0c-145">top</span><span class="sxs-lookup"><span data-stu-id="36f0c-145">top</span></span>|<span data-ttu-id="36f0c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="36f0c-146">Int32</span></span>|<span data-ttu-id="36f0c-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-147">Not yet documented</span></span>|
|<span data-ttu-id="36f0c-148">skip</span><span class="sxs-lookup"><span data-stu-id="36f0c-148">skip</span></span>|<span data-ttu-id="36f0c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="36f0c-149">Int32</span></span>|<span data-ttu-id="36f0c-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36f0c-150">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="36f0c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="36f0c-151">Response</span></span>
<span data-ttu-id="36f0c-152">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [назначениеFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="36f0c-152">If successful, this action returns a `200 OK` response code and a [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f0c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="36f0c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="36f0c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="36f0c-154">Request</span></span>
<span data-ttu-id="36f0c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36f0c-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/getAssignmentFiltersStatusDetails

Content-type: application/json
Content-length: 214

{
  "managedDeviceId": "Managed Device Id value",
  "payloadId": "Payload Id value",
  "userId": "User Id value",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ],
  "top": 3,
  "skip": 4
}
```

### <a name="response"></a><span data-ttu-id="36f0c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f0c-156">Response</span></span>
<span data-ttu-id="36f0c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36f0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterStatusDetails",
    "managedDeviceId": "Managed Device Id value",
    "payloadId": "Payload Id value",
    "userId": "User Id value",
    "deviceProperties": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "evalutionSummaries": [
      {
        "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
        "assignmentFilterId": "Assignment Filter Id value",
        "assignmentFilterLastModifiedDateTime": "2017-01-01T00:02:50.0900701-08:00",
        "assignmentFilterDisplayName": "Assignment Filter Display Name value",
        "assignmentFilterPlatform": "androidForWork",
        "evaluationResult": "match",
        "evaluationDateTime": "2016-12-31T23:58:01.2047675-08:00",
        "assignmentFilterType": "include",
        "assignmentFilterTypeAndEvaluationResults": [
          {
            "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
            "assignmentFilterType": "include",
            "evaluationResult": "match"
          }
        ]
      }
    ]
  }
}
```




