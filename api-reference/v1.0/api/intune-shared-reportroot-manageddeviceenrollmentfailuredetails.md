---
title: функция managedDeviceEnrollmentFailureDetails
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 128ad6e3985649b3dbaffa101c19f0b2440b0838
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980379"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="18c13-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="18c13-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="18c13-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18c13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18c13-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18c13-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18c13-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18c13-106">Prerequisites</span></span>
<span data-ttu-id="18c13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18c13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18c13-109">Permission type</span></span>|<span data-ttu-id="18c13-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18c13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18c13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18c13-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="18c13-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="18c13-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="18c13-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18c13-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="18c13-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18c13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18c13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c13-115">Not supported.</span></span>|
|<span data-ttu-id="18c13-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18c13-116">Application</span></span>|<span data-ttu-id="18c13-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18c13-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18c13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="18c13-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18c13-119">Request headers</span></span>
|<span data-ttu-id="18c13-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18c13-120">Header</span></span>|<span data-ttu-id="18c13-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18c13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18c13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18c13-122">Authorization</span></span>|<span data-ttu-id="18c13-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18c13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18c13-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18c13-124">Accept</span></span>|<span data-ttu-id="18c13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18c13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18c13-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18c13-126">Request body</span></span>
<span data-ttu-id="18c13-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="18c13-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="18c13-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="18c13-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="18c13-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18c13-129">Property</span></span>|<span data-ttu-id="18c13-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18c13-130">Type</span></span>|<span data-ttu-id="18c13-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18c13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18c13-132">skip</span><span class="sxs-lookup"><span data-stu-id="18c13-132">skip</span></span>|<span data-ttu-id="18c13-133">Int32</span><span class="sxs-lookup"><span data-stu-id="18c13-133">Int32</span></span>|<span data-ttu-id="18c13-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18c13-134">Not yet documented</span></span>|
|<span data-ttu-id="18c13-135">top</span><span class="sxs-lookup"><span data-stu-id="18c13-135">top</span></span>|<span data-ttu-id="18c13-136">Int32</span><span class="sxs-lookup"><span data-stu-id="18c13-136">Int32</span></span>|<span data-ttu-id="18c13-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18c13-137">Not yet documented</span></span>|
|<span data-ttu-id="18c13-138">filter</span><span class="sxs-lookup"><span data-stu-id="18c13-138">filter</span></span>|<span data-ttu-id="18c13-139">String</span><span class="sxs-lookup"><span data-stu-id="18c13-139">String</span></span>|<span data-ttu-id="18c13-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18c13-140">Not yet documented</span></span>|
|<span data-ttu-id="18c13-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="18c13-141">skipToken</span></span>|<span data-ttu-id="18c13-142">String</span><span class="sxs-lookup"><span data-stu-id="18c13-142">String</span></span>|<span data-ttu-id="18c13-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18c13-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="18c13-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="18c13-144">Response</span></span>
<span data-ttu-id="18c13-145">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18c13-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18c13-146">Пример</span><span class="sxs-lookup"><span data-stu-id="18c13-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="18c13-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="18c13-147">Request</span></span>
<span data-ttu-id="18c13-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18c13-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="18c13-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="18c13-149">Response</span></span>
<span data-ttu-id="18c13-150">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="18c13-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="18c13-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18c13-151">All of the properties will be returned from an actual call.</span></span>

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




