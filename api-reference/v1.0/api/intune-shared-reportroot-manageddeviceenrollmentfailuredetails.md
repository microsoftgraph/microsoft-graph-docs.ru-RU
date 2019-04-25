---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c234181bb70ca0df11cff01b67eb7d6fa60e27ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576799"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="3006a-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="3006a-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="3006a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3006a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3006a-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3006a-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3006a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3006a-106">Prerequisites</span></span>
<span data-ttu-id="3006a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3006a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3006a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3006a-109">Permission type</span></span>|<span data-ttu-id="3006a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3006a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3006a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3006a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3006a-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3006a-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3006a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3006a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3006a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3006a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3006a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3006a-115">Not supported.</span></span>|
|<span data-ttu-id="3006a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3006a-116">Application</span></span>|<span data-ttu-id="3006a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3006a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3006a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3006a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="3006a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3006a-119">Request headers</span></span>
|<span data-ttu-id="3006a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3006a-120">Header</span></span>|<span data-ttu-id="3006a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3006a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3006a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3006a-122">Authorization</span></span>|<span data-ttu-id="3006a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3006a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3006a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3006a-124">Accept</span></span>|<span data-ttu-id="3006a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3006a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3006a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3006a-126">Request body</span></span>
<span data-ttu-id="3006a-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="3006a-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3006a-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="3006a-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3006a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3006a-129">Property</span></span>|<span data-ttu-id="3006a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3006a-130">Type</span></span>|<span data-ttu-id="3006a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3006a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3006a-132">skip</span><span class="sxs-lookup"><span data-stu-id="3006a-132">skip</span></span>|<span data-ttu-id="3006a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3006a-133">Int32</span></span>|<span data-ttu-id="3006a-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3006a-134">Not yet documented</span></span>|
|<span data-ttu-id="3006a-135">top</span><span class="sxs-lookup"><span data-stu-id="3006a-135">top</span></span>|<span data-ttu-id="3006a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3006a-136">Int32</span></span>|<span data-ttu-id="3006a-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3006a-137">Not yet documented</span></span>|
|<span data-ttu-id="3006a-138">filter</span><span class="sxs-lookup"><span data-stu-id="3006a-138">filter</span></span>|<span data-ttu-id="3006a-139">String</span><span class="sxs-lookup"><span data-stu-id="3006a-139">String</span></span>|<span data-ttu-id="3006a-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3006a-140">Not yet documented</span></span>|
|<span data-ttu-id="3006a-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="3006a-141">skipToken</span></span>|<span data-ttu-id="3006a-142">String</span><span class="sxs-lookup"><span data-stu-id="3006a-142">String</span></span>|<span data-ttu-id="3006a-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3006a-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3006a-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="3006a-144">Response</span></span>
<span data-ttu-id="3006a-145">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3006a-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3006a-146">Пример</span><span class="sxs-lookup"><span data-stu-id="3006a-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="3006a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3006a-147">Request</span></span>
<span data-ttu-id="3006a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3006a-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3006a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3006a-149">Response</span></span>
<span data-ttu-id="3006a-150">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3006a-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3006a-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3006a-151">All of the properties will be returned from an actual call.</span></span>

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




