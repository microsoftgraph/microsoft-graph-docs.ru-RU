---
title: функция managedDeviceEnrollmentTopFailures
description: Н/Д
ms.openlocfilehash: 2fb1fc9d611f4a61cf243de0d1c44fa2a3da889e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028327"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="7cda1-103">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="7cda1-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="7cda1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7cda1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cda1-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7cda1-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cda1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7cda1-106">Prerequisites</span></span>
<span data-ttu-id="7cda1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cda1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cda1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cda1-109">Permission type</span></span>|<span data-ttu-id="7cda1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cda1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cda1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cda1-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7cda1-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="7cda1-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7cda1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cda1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7cda1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cda1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cda1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cda1-115">Not supported.</span></span>|
|<span data-ttu-id="7cda1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cda1-116">Application</span></span>|<span data-ttu-id="7cda1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cda1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cda1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cda1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="7cda1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cda1-119">Request headers</span></span>
|<span data-ttu-id="7cda1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cda1-120">Header</span></span>|<span data-ttu-id="7cda1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7cda1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cda1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cda1-122">Authorization</span></span>|<span data-ttu-id="7cda1-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7cda1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cda1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7cda1-124">Accept</span></span>|<span data-ttu-id="7cda1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cda1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cda1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cda1-126">Request body</span></span>
<span data-ttu-id="7cda1-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7cda1-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7cda1-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="7cda1-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7cda1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cda1-129">Property</span></span>|<span data-ttu-id="7cda1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7cda1-130">Type</span></span>|<span data-ttu-id="7cda1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7cda1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cda1-132">period</span><span class="sxs-lookup"><span data-stu-id="7cda1-132">period</span></span>|<span data-ttu-id="7cda1-133">String</span><span class="sxs-lookup"><span data-stu-id="7cda1-133">String</span></span>|<span data-ttu-id="7cda1-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7cda1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7cda1-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cda1-135">Response</span></span>
<span data-ttu-id="7cda1-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cda1-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cda1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7cda1-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cda1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cda1-138">Request</span></span>
<span data-ttu-id="7cda1-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cda1-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7cda1-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cda1-140">Response</span></span>
<span data-ttu-id="7cda1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7cda1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




