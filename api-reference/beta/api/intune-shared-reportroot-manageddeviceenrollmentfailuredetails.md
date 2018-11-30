---
title: функция managedDeviceEnrollmentFailureDetails
description: Н/Д
ms.openlocfilehash: 92a06a4fae5d469759f633698abcf7bff2bfb322
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079063"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="8b97a-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="8b97a-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="8b97a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b97a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b97a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b97a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b97a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b97a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b97a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b97a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b97a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b97a-108">Prerequisites</span></span>
<span data-ttu-id="8b97a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b97a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b97a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b97a-111">Permission type</span></span>|<span data-ttu-id="8b97a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b97a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b97a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b97a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8b97a-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="8b97a-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8b97a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b97a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8b97a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b97a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b97a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b97a-117">Not supported.</span></span>|
|<span data-ttu-id="8b97a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b97a-118">Application</span></span>|<span data-ttu-id="8b97a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b97a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b97a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b97a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="8b97a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b97a-121">Request headers</span></span>
|<span data-ttu-id="8b97a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b97a-122">Header</span></span>|<span data-ttu-id="8b97a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8b97a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b97a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b97a-124">Authorization</span></span>|<span data-ttu-id="8b97a-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8b97a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b97a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8b97a-126">Accept</span></span>|<span data-ttu-id="8b97a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8b97a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b97a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b97a-128">Request body</span></span>
<span data-ttu-id="8b97a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8b97a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8b97a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b97a-130">Property</span></span>|<span data-ttu-id="8b97a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b97a-131">Type</span></span>|<span data-ttu-id="8b97a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b97a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b97a-133">filter</span><span class="sxs-lookup"><span data-stu-id="8b97a-133">filter</span></span>|<span data-ttu-id="8b97a-134">String</span><span class="sxs-lookup"><span data-stu-id="8b97a-134">String</span></span>|<span data-ttu-id="8b97a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b97a-135">Not yet documented</span></span>|
|<span data-ttu-id="8b97a-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="8b97a-136">skipToken</span></span>|<span data-ttu-id="8b97a-137">String</span><span class="sxs-lookup"><span data-stu-id="8b97a-137">String</span></span>|<span data-ttu-id="8b97a-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b97a-138">Not yet documented</span></span>|
|<span data-ttu-id="8b97a-139">skip</span><span class="sxs-lookup"><span data-stu-id="8b97a-139">skip</span></span>|<span data-ttu-id="8b97a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8b97a-140">Int32</span></span>|<span data-ttu-id="8b97a-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b97a-141">Not yet documented</span></span>|
|<span data-ttu-id="8b97a-142">top</span><span class="sxs-lookup"><span data-stu-id="8b97a-142">top</span></span>|<span data-ttu-id="8b97a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8b97a-143">Int32</span></span>|<span data-ttu-id="8b97a-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b97a-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8b97a-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b97a-145">Response</span></span>
<span data-ttu-id="8b97a-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b97a-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b97a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8b97a-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b97a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b97a-148">Request</span></span>
<span data-ttu-id="8b97a-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b97a-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8b97a-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b97a-150">Response</span></span>
<span data-ttu-id="8b97a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8b97a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



