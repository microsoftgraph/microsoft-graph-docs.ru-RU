---
title: функция managedDeviceEnrollmentTopFailures
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 163a75a2ffa675f939086fecf3e9c4a155352aa1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934228"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="66586-103">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="66586-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="66586-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66586-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66586-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66586-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66586-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66586-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66586-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66586-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66586-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="66586-108">Prerequisites</span></span>
<span data-ttu-id="66586-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66586-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66586-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66586-111">Permission type</span></span>|<span data-ttu-id="66586-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66586-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66586-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66586-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="66586-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="66586-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="66586-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66586-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="66586-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66586-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66586-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66586-117">Not supported.</span></span>|
|<span data-ttu-id="66586-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66586-118">Application</span></span>|<span data-ttu-id="66586-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66586-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66586-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66586-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="66586-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66586-121">Request headers</span></span>
|<span data-ttu-id="66586-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66586-122">Header</span></span>|<span data-ttu-id="66586-123">Значение</span><span class="sxs-lookup"><span data-stu-id="66586-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66586-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="66586-124">Authorization</span></span>|<span data-ttu-id="66586-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66586-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66586-126">Accept</span><span class="sxs-lookup"><span data-stu-id="66586-126">Accept</span></span>|<span data-ttu-id="66586-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66586-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66586-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66586-128">Request body</span></span>
<span data-ttu-id="66586-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="66586-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="66586-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="66586-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="66586-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="66586-131">Property</span></span>|<span data-ttu-id="66586-132">Тип</span><span class="sxs-lookup"><span data-stu-id="66586-132">Type</span></span>|<span data-ttu-id="66586-133">Описание</span><span class="sxs-lookup"><span data-stu-id="66586-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66586-134">period</span><span class="sxs-lookup"><span data-stu-id="66586-134">period</span></span>|<span data-ttu-id="66586-135">Строка</span><span class="sxs-lookup"><span data-stu-id="66586-135">String</span></span>|<span data-ttu-id="66586-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66586-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66586-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="66586-137">Response</span></span>
<span data-ttu-id="66586-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66586-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66586-139">Пример</span><span class="sxs-lookup"><span data-stu-id="66586-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="66586-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="66586-140">Request</span></span>
<span data-ttu-id="66586-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66586-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="66586-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="66586-142">Response</span></span>
<span data-ttu-id="66586-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66586-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



