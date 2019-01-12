---
title: функция managedDeviceEnrollmentAbandonmentSummary
description: Метаданные для регистрации abandonment сводного отчета
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c4ea4a3cefe862193557928f8865d79c0716329
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930707"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="96d5b-103">функция managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="96d5b-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="96d5b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96d5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96d5b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96d5b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96d5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96d5b-107">Метаданные для регистрации abandonment сводного отчета</span><span class="sxs-lookup"><span data-stu-id="96d5b-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96d5b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96d5b-108">Prerequisites</span></span>
<span data-ttu-id="96d5b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d5b-111">Permission type</span></span>|<span data-ttu-id="96d5b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d5b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d5b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="96d5b-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="96d5b-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="96d5b-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="96d5b-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="96d5b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d5b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d5b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d5b-117">Not supported.</span></span>|
|<span data-ttu-id="96d5b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96d5b-118">Application</span></span>|<span data-ttu-id="96d5b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d5b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96d5b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d5b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="96d5b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96d5b-121">Request headers</span></span>
|<span data-ttu-id="96d5b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96d5b-122">Header</span></span>|<span data-ttu-id="96d5b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="96d5b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96d5b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d5b-124">Authorization</span></span>|<span data-ttu-id="96d5b-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="96d5b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96d5b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="96d5b-126">Accept</span></span>|<span data-ttu-id="96d5b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="96d5b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d5b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96d5b-128">Request body</span></span>
<span data-ttu-id="96d5b-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="96d5b-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="96d5b-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="96d5b-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="96d5b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="96d5b-131">Property</span></span>|<span data-ttu-id="96d5b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="96d5b-132">Type</span></span>|<span data-ttu-id="96d5b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="96d5b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96d5b-134">skip</span><span class="sxs-lookup"><span data-stu-id="96d5b-134">skip</span></span>|<span data-ttu-id="96d5b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="96d5b-135">Int32</span></span>|<span data-ttu-id="96d5b-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="96d5b-136">Not yet documented</span></span>|
|<span data-ttu-id="96d5b-137">top</span><span class="sxs-lookup"><span data-stu-id="96d5b-137">top</span></span>|<span data-ttu-id="96d5b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="96d5b-138">Int32</span></span>|<span data-ttu-id="96d5b-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="96d5b-139">Not yet documented</span></span>|
|<span data-ttu-id="96d5b-140">filter</span><span class="sxs-lookup"><span data-stu-id="96d5b-140">filter</span></span>|<span data-ttu-id="96d5b-141">String</span><span class="sxs-lookup"><span data-stu-id="96d5b-141">String</span></span>|<span data-ttu-id="96d5b-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="96d5b-142">Not yet documented</span></span>|
|<span data-ttu-id="96d5b-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="96d5b-143">skipToken</span></span>|<span data-ttu-id="96d5b-144">String</span><span class="sxs-lookup"><span data-stu-id="96d5b-144">String</span></span>|<span data-ttu-id="96d5b-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="96d5b-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="96d5b-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="96d5b-146">Response</span></span>
<span data-ttu-id="96d5b-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96d5b-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d5b-148">Пример</span><span class="sxs-lookup"><span data-stu-id="96d5b-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="96d5b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d5b-149">Request</span></span>
<span data-ttu-id="96d5b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d5b-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="96d5b-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="96d5b-151">Response</span></span>
<span data-ttu-id="96d5b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96d5b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





