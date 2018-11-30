---
title: функция managedDeviceEnrollmentFailureDetails
description: Н/Д
ms.openlocfilehash: c5e68453cb1655e4018156ac207b60e4145e571a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027448"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="77bdd-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="77bdd-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="77bdd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="77bdd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77bdd-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77bdd-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77bdd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77bdd-106">Prerequisites</span></span>
<span data-ttu-id="77bdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77bdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77bdd-109">Permission type</span></span>|<span data-ttu-id="77bdd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77bdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77bdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77bdd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="77bdd-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="77bdd-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="77bdd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77bdd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77bdd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77bdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77bdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77bdd-115">Not supported.</span></span>|
|<span data-ttu-id="77bdd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77bdd-116">Application</span></span>|<span data-ttu-id="77bdd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77bdd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77bdd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77bdd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="77bdd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77bdd-119">Request headers</span></span>
|<span data-ttu-id="77bdd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77bdd-120">Header</span></span>|<span data-ttu-id="77bdd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77bdd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77bdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77bdd-122">Authorization</span></span>|<span data-ttu-id="77bdd-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77bdd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77bdd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="77bdd-124">Accept</span></span>|<span data-ttu-id="77bdd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77bdd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77bdd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77bdd-126">Request body</span></span>
<span data-ttu-id="77bdd-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="77bdd-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="77bdd-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="77bdd-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="77bdd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77bdd-129">Property</span></span>|<span data-ttu-id="77bdd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77bdd-130">Type</span></span>|<span data-ttu-id="77bdd-131">Description</span><span class="sxs-lookup"><span data-stu-id="77bdd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77bdd-132">skip</span><span class="sxs-lookup"><span data-stu-id="77bdd-132">skip</span></span>|<span data-ttu-id="77bdd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="77bdd-133">Int32</span></span>|<span data-ttu-id="77bdd-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77bdd-134">Not yet documented</span></span>|
|<span data-ttu-id="77bdd-135">top</span><span class="sxs-lookup"><span data-stu-id="77bdd-135">top</span></span>|<span data-ttu-id="77bdd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="77bdd-136">Int32</span></span>|<span data-ttu-id="77bdd-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77bdd-137">Not yet documented</span></span>|
|<span data-ttu-id="77bdd-138">filter</span><span class="sxs-lookup"><span data-stu-id="77bdd-138">filter</span></span>|<span data-ttu-id="77bdd-139">String</span><span class="sxs-lookup"><span data-stu-id="77bdd-139">String</span></span>|<span data-ttu-id="77bdd-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77bdd-140">Not yet documented</span></span>|
|<span data-ttu-id="77bdd-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="77bdd-141">skipToken</span></span>|<span data-ttu-id="77bdd-142">String</span><span class="sxs-lookup"><span data-stu-id="77bdd-142">String</span></span>|<span data-ttu-id="77bdd-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77bdd-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="77bdd-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="77bdd-144">Response</span></span>
<span data-ttu-id="77bdd-145">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77bdd-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77bdd-146">Пример</span><span class="sxs-lookup"><span data-stu-id="77bdd-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="77bdd-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="77bdd-147">Request</span></span>
<span data-ttu-id="77bdd-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77bdd-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="77bdd-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="77bdd-149">Response</span></span>
<span data-ttu-id="77bdd-150">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="77bdd-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77bdd-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77bdd-151">All of the properties will be returned from an actual call.</span></span>

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




