---
title: функция managedDeviceEnrollmentFailureDetails
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7e3ad342ad19314e10ae5e2987143646e5796c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840371"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="2761b-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="2761b-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="2761b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2761b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2761b-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2761b-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2761b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2761b-106">Prerequisites</span></span>
<span data-ttu-id="2761b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2761b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2761b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2761b-109">Permission type</span></span>|<span data-ttu-id="2761b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2761b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2761b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2761b-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2761b-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="2761b-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="2761b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2761b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2761b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2761b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2761b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2761b-115">Not supported.</span></span>|
|<span data-ttu-id="2761b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2761b-116">Application</span></span>|<span data-ttu-id="2761b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2761b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2761b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2761b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="2761b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2761b-119">Request headers</span></span>
|<span data-ttu-id="2761b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2761b-120">Header</span></span>|<span data-ttu-id="2761b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2761b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2761b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2761b-122">Authorization</span></span>|<span data-ttu-id="2761b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2761b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2761b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2761b-124">Accept</span></span>|<span data-ttu-id="2761b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2761b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2761b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2761b-126">Request body</span></span>
<span data-ttu-id="2761b-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="2761b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2761b-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="2761b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2761b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2761b-129">Property</span></span>|<span data-ttu-id="2761b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2761b-130">Type</span></span>|<span data-ttu-id="2761b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2761b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2761b-132">skip</span><span class="sxs-lookup"><span data-stu-id="2761b-132">skip</span></span>|<span data-ttu-id="2761b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2761b-133">Int32</span></span>|<span data-ttu-id="2761b-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2761b-134">Not yet documented</span></span>|
|<span data-ttu-id="2761b-135">top</span><span class="sxs-lookup"><span data-stu-id="2761b-135">top</span></span>|<span data-ttu-id="2761b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2761b-136">Int32</span></span>|<span data-ttu-id="2761b-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2761b-137">Not yet documented</span></span>|
|<span data-ttu-id="2761b-138">filter</span><span class="sxs-lookup"><span data-stu-id="2761b-138">filter</span></span>|<span data-ttu-id="2761b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="2761b-139">String</span></span>|<span data-ttu-id="2761b-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2761b-140">Not yet documented</span></span>|
|<span data-ttu-id="2761b-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="2761b-141">skipToken</span></span>|<span data-ttu-id="2761b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2761b-142">String</span></span>|<span data-ttu-id="2761b-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2761b-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2761b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="2761b-144">Response</span></span>
<span data-ttu-id="2761b-145">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2761b-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2761b-146">Пример</span><span class="sxs-lookup"><span data-stu-id="2761b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2761b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="2761b-147">Request</span></span>
<span data-ttu-id="2761b-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2761b-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2761b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="2761b-149">Response</span></span>
<span data-ttu-id="2761b-150">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="2761b-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2761b-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2761b-151">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




