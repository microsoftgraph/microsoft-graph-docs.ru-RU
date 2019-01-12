---
title: функция managedDeviceEnrollmentTopFailures
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4a21d9fc0b29c63053d184db235a1c44744d8e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932660"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="16135-103">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="16135-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="16135-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16135-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16135-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16135-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16135-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="16135-106">Prerequisites</span></span>
<span data-ttu-id="16135-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16135-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16135-109">Permission type</span></span>|<span data-ttu-id="16135-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16135-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16135-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16135-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="16135-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="16135-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="16135-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16135-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="16135-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16135-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16135-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16135-115">Not supported.</span></span>|
|<span data-ttu-id="16135-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16135-116">Application</span></span>|<span data-ttu-id="16135-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16135-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16135-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16135-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="16135-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16135-119">Request headers</span></span>
|<span data-ttu-id="16135-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16135-120">Header</span></span>|<span data-ttu-id="16135-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16135-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16135-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16135-122">Authorization</span></span>|<span data-ttu-id="16135-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16135-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16135-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16135-124">Accept</span></span>|<span data-ttu-id="16135-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16135-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16135-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16135-126">Request body</span></span>
<span data-ttu-id="16135-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="16135-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="16135-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="16135-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="16135-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="16135-129">Property</span></span>|<span data-ttu-id="16135-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16135-130">Type</span></span>|<span data-ttu-id="16135-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16135-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16135-132">period</span><span class="sxs-lookup"><span data-stu-id="16135-132">period</span></span>|<span data-ttu-id="16135-133">Строка</span><span class="sxs-lookup"><span data-stu-id="16135-133">String</span></span>|<span data-ttu-id="16135-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16135-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="16135-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="16135-135">Response</span></span>
<span data-ttu-id="16135-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16135-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16135-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16135-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="16135-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="16135-138">Request</span></span>
<span data-ttu-id="16135-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16135-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="16135-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="16135-140">Response</span></span>
<span data-ttu-id="16135-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16135-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




