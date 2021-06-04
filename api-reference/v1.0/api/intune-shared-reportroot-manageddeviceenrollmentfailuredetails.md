---
title: функция managedDeviceEnrollmentFailureDetails
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1539992ad475c2339a33aae809bc477d5da4e772
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732754"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="e0506-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="e0506-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="e0506-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0506-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0506-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0506-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0506-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e0506-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0506-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0506-107">Prerequisites</span></span>
<span data-ttu-id="e0506-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0506-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0506-110">Permission type</span></span>|<span data-ttu-id="e0506-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0506-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0506-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0506-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e0506-113">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e0506-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e0506-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0506-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e0506-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0506-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0506-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0506-116">Not supported.</span></span>|
|<span data-ttu-id="e0506-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0506-117">Application</span></span>|<span data-ttu-id="e0506-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0506-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0506-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0506-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="e0506-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0506-120">Request headers</span></span>
|<span data-ttu-id="e0506-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0506-121">Header</span></span>|<span data-ttu-id="e0506-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0506-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0506-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0506-123">Authorization</span></span>|<span data-ttu-id="e0506-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0506-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0506-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0506-125">Accept</span></span>|<span data-ttu-id="e0506-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0506-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0506-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0506-127">Request body</span></span>
<span data-ttu-id="e0506-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e0506-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e0506-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="e0506-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e0506-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0506-130">Property</span></span>|<span data-ttu-id="e0506-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0506-131">Type</span></span>|<span data-ttu-id="e0506-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0506-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0506-133">skip</span><span class="sxs-lookup"><span data-stu-id="e0506-133">skip</span></span>|<span data-ttu-id="e0506-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e0506-134">Int32</span></span>|<span data-ttu-id="e0506-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e0506-135">Not yet documented</span></span>|
|<span data-ttu-id="e0506-136">top</span><span class="sxs-lookup"><span data-stu-id="e0506-136">top</span></span>|<span data-ttu-id="e0506-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e0506-137">Int32</span></span>|<span data-ttu-id="e0506-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e0506-138">Not yet documented</span></span>|
|<span data-ttu-id="e0506-139">filter</span><span class="sxs-lookup"><span data-stu-id="e0506-139">filter</span></span>|<span data-ttu-id="e0506-140">String</span><span class="sxs-lookup"><span data-stu-id="e0506-140">String</span></span>|<span data-ttu-id="e0506-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e0506-141">Not yet documented</span></span>|
|<span data-ttu-id="e0506-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="e0506-142">skipToken</span></span>|<span data-ttu-id="e0506-143">String</span><span class="sxs-lookup"><span data-stu-id="e0506-143">String</span></span>|<span data-ttu-id="e0506-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e0506-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e0506-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0506-145">Response</span></span>
<span data-ttu-id="e0506-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0506-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0506-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e0506-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0506-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0506-148">Request</span></span>
<span data-ttu-id="e0506-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0506-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e0506-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0506-150">Response</span></span>
<span data-ttu-id="e0506-151">Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e0506-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0506-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0506-152">All of the properties will be returned from an actual call.</span></span>

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










