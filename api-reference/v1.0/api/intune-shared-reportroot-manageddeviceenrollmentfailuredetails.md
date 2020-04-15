---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b28adb643367b9bdc31b08e78bacceae48642422
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411580"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="03384-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="03384-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="03384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03384-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03384-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03384-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03384-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="03384-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03384-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="03384-107">Prerequisites</span></span>
<span data-ttu-id="03384-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03384-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03384-110">Permission type</span></span>|<span data-ttu-id="03384-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03384-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03384-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03384-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="03384-113">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="03384-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="03384-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03384-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03384-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03384-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03384-116">Not supported.</span></span>|
|<span data-ttu-id="03384-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03384-117">Application</span></span>|<span data-ttu-id="03384-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03384-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03384-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03384-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="03384-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03384-120">Request headers</span></span>
|<span data-ttu-id="03384-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03384-121">Header</span></span>|<span data-ttu-id="03384-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03384-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03384-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03384-123">Authorization</span></span>|<span data-ttu-id="03384-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03384-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03384-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03384-125">Accept</span></span>|<span data-ttu-id="03384-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03384-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03384-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03384-127">Request body</span></span>
<span data-ttu-id="03384-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="03384-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="03384-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="03384-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="03384-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03384-130">Property</span></span>|<span data-ttu-id="03384-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03384-131">Type</span></span>|<span data-ttu-id="03384-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03384-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03384-133">skip</span><span class="sxs-lookup"><span data-stu-id="03384-133">skip</span></span>|<span data-ttu-id="03384-134">Int32</span><span class="sxs-lookup"><span data-stu-id="03384-134">Int32</span></span>|<span data-ttu-id="03384-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="03384-135">Not yet documented</span></span>|
|<span data-ttu-id="03384-136">top</span><span class="sxs-lookup"><span data-stu-id="03384-136">top</span></span>|<span data-ttu-id="03384-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03384-137">Int32</span></span>|<span data-ttu-id="03384-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="03384-138">Not yet documented</span></span>|
|<span data-ttu-id="03384-139">filter</span><span class="sxs-lookup"><span data-stu-id="03384-139">filter</span></span>|<span data-ttu-id="03384-140">String</span><span class="sxs-lookup"><span data-stu-id="03384-140">String</span></span>|<span data-ttu-id="03384-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="03384-141">Not yet documented</span></span>|
|<span data-ttu-id="03384-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="03384-142">skipToken</span></span>|<span data-ttu-id="03384-143">String</span><span class="sxs-lookup"><span data-stu-id="03384-143">String</span></span>|<span data-ttu-id="03384-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="03384-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="03384-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="03384-145">Response</span></span>
<span data-ttu-id="03384-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03384-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03384-147">Пример</span><span class="sxs-lookup"><span data-stu-id="03384-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="03384-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="03384-148">Request</span></span>
<span data-ttu-id="03384-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03384-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="03384-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="03384-150">Response</span></span>
<span data-ttu-id="03384-151">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="03384-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="03384-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03384-152">All of the properties will be returned from an actual call.</span></span>

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







