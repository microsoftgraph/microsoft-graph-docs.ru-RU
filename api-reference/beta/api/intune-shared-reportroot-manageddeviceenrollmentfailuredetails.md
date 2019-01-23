---
title: функция managedDeviceEnrollmentFailureDetails
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e861b8947396c67c72ba47493d30e6010905b107
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415560"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="945a0-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="945a0-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="945a0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="945a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="945a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="945a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="945a0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="945a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="945a0-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945a0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="945a0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="945a0-108">Prerequisites</span></span>
<span data-ttu-id="945a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="945a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="945a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="945a0-111">Permission type</span></span>|<span data-ttu-id="945a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="945a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="945a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="945a0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="945a0-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="945a0-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="945a0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="945a0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="945a0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="945a0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="945a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="945a0-117">Not supported.</span></span>|
|<span data-ttu-id="945a0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="945a0-118">Application</span></span>|<span data-ttu-id="945a0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="945a0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="945a0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="945a0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="945a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="945a0-121">Request headers</span></span>
|<span data-ttu-id="945a0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="945a0-122">Header</span></span>|<span data-ttu-id="945a0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="945a0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="945a0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="945a0-124">Authorization</span></span>|<span data-ttu-id="945a0-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="945a0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="945a0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="945a0-126">Accept</span></span>|<span data-ttu-id="945a0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="945a0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="945a0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="945a0-128">Request body</span></span>
<span data-ttu-id="945a0-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="945a0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="945a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="945a0-130">Property</span></span>|<span data-ttu-id="945a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="945a0-131">Type</span></span>|<span data-ttu-id="945a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="945a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="945a0-133">filter</span><span class="sxs-lookup"><span data-stu-id="945a0-133">filter</span></span>|<span data-ttu-id="945a0-134">String</span><span class="sxs-lookup"><span data-stu-id="945a0-134">String</span></span>|<span data-ttu-id="945a0-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945a0-135">Not yet documented</span></span>|
|<span data-ttu-id="945a0-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="945a0-136">skipToken</span></span>|<span data-ttu-id="945a0-137">String</span><span class="sxs-lookup"><span data-stu-id="945a0-137">String</span></span>|<span data-ttu-id="945a0-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945a0-138">Not yet documented</span></span>|
|<span data-ttu-id="945a0-139">skip</span><span class="sxs-lookup"><span data-stu-id="945a0-139">skip</span></span>|<span data-ttu-id="945a0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="945a0-140">Int32</span></span>|<span data-ttu-id="945a0-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945a0-141">Not yet documented</span></span>|
|<span data-ttu-id="945a0-142">top</span><span class="sxs-lookup"><span data-stu-id="945a0-142">top</span></span>|<span data-ttu-id="945a0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="945a0-143">Int32</span></span>|<span data-ttu-id="945a0-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="945a0-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="945a0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="945a0-145">Response</span></span>
<span data-ttu-id="945a0-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="945a0-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="945a0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="945a0-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="945a0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="945a0-148">Request</span></span>
<span data-ttu-id="945a0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="945a0-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="945a0-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="945a0-150">Response</span></span>
<span data-ttu-id="945a0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="945a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



