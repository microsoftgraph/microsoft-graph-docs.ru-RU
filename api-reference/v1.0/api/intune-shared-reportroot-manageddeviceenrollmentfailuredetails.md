---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da38aa1fb497bc5fb1225f2435ed2bd9c4e4b3c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025850"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="fe10f-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="fe10f-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="fe10f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe10f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe10f-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fe10f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe10f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe10f-106">Prerequisites</span></span>
<span data-ttu-id="fe10f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe10f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe10f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe10f-109">Permission type</span></span>|<span data-ttu-id="fe10f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe10f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe10f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe10f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe10f-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="fe10f-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="fe10f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe10f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe10f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe10f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe10f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe10f-115">Not supported.</span></span>|
|<span data-ttu-id="fe10f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe10f-116">Application</span></span>|<span data-ttu-id="fe10f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe10f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe10f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe10f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="fe10f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe10f-119">Request headers</span></span>
|<span data-ttu-id="fe10f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe10f-120">Header</span></span>|<span data-ttu-id="fe10f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe10f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe10f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe10f-122">Authorization</span></span>|<span data-ttu-id="fe10f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe10f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe10f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe10f-124">Accept</span></span>|<span data-ttu-id="fe10f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe10f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe10f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe10f-126">Request body</span></span>
<span data-ttu-id="fe10f-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fe10f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fe10f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fe10f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fe10f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe10f-129">Property</span></span>|<span data-ttu-id="fe10f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe10f-130">Type</span></span>|<span data-ttu-id="fe10f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe10f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe10f-132">skip</span><span class="sxs-lookup"><span data-stu-id="fe10f-132">skip</span></span>|<span data-ttu-id="fe10f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="fe10f-133">Int32</span></span>|<span data-ttu-id="fe10f-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fe10f-134">Not yet documented</span></span>|
|<span data-ttu-id="fe10f-135">top</span><span class="sxs-lookup"><span data-stu-id="fe10f-135">top</span></span>|<span data-ttu-id="fe10f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fe10f-136">Int32</span></span>|<span data-ttu-id="fe10f-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fe10f-137">Not yet documented</span></span>|
|<span data-ttu-id="fe10f-138">filter</span><span class="sxs-lookup"><span data-stu-id="fe10f-138">filter</span></span>|<span data-ttu-id="fe10f-139">String</span><span class="sxs-lookup"><span data-stu-id="fe10f-139">String</span></span>|<span data-ttu-id="fe10f-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fe10f-140">Not yet documented</span></span>|
|<span data-ttu-id="fe10f-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="fe10f-141">skipToken</span></span>|<span data-ttu-id="fe10f-142">String</span><span class="sxs-lookup"><span data-stu-id="fe10f-142">String</span></span>|<span data-ttu-id="fe10f-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fe10f-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fe10f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe10f-144">Response</span></span>
<span data-ttu-id="fe10f-145">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe10f-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe10f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="fe10f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe10f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe10f-147">Request</span></span>
<span data-ttu-id="fe10f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe10f-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fe10f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe10f-149">Response</span></span>
<span data-ttu-id="fe10f-150">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fe10f-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe10f-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe10f-151">All of the properties will be returned from an actual call.</span></span>

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




