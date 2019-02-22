---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9521a2265e6fcdb86b60d6fc427c74d74be0b31f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164381"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="22328-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="22328-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="22328-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22328-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22328-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22328-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22328-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22328-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22328-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="22328-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22328-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="22328-108">Prerequisites</span></span>
<span data-ttu-id="22328-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22328-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="22328-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22328-111">Permission type</span></span>|<span data-ttu-id="22328-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22328-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22328-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22328-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="22328-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="22328-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="22328-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22328-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="22328-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22328-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22328-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22328-117">Not supported.</span></span>|
|<span data-ttu-id="22328-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22328-118">Application</span></span>|<span data-ttu-id="22328-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22328-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22328-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22328-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="22328-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22328-121">Request headers</span></span>
|<span data-ttu-id="22328-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22328-122">Header</span></span>|<span data-ttu-id="22328-123">Значение</span><span class="sxs-lookup"><span data-stu-id="22328-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22328-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22328-124">Authorization</span></span>|<span data-ttu-id="22328-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22328-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22328-126">Accept</span><span class="sxs-lookup"><span data-stu-id="22328-126">Accept</span></span>|<span data-ttu-id="22328-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22328-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22328-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22328-128">Request body</span></span>
<span data-ttu-id="22328-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="22328-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="22328-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22328-130">Property</span></span>|<span data-ttu-id="22328-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22328-131">Type</span></span>|<span data-ttu-id="22328-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22328-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22328-133">filter</span><span class="sxs-lookup"><span data-stu-id="22328-133">filter</span></span>|<span data-ttu-id="22328-134">String</span><span class="sxs-lookup"><span data-stu-id="22328-134">String</span></span>|<span data-ttu-id="22328-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22328-135">Not yet documented</span></span>|
|<span data-ttu-id="22328-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="22328-136">skipToken</span></span>|<span data-ttu-id="22328-137">String</span><span class="sxs-lookup"><span data-stu-id="22328-137">String</span></span>|<span data-ttu-id="22328-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22328-138">Not yet documented</span></span>|
|<span data-ttu-id="22328-139">skip</span><span class="sxs-lookup"><span data-stu-id="22328-139">skip</span></span>|<span data-ttu-id="22328-140">Int32</span><span class="sxs-lookup"><span data-stu-id="22328-140">Int32</span></span>|<span data-ttu-id="22328-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22328-141">Not yet documented</span></span>|
|<span data-ttu-id="22328-142">top</span><span class="sxs-lookup"><span data-stu-id="22328-142">top</span></span>|<span data-ttu-id="22328-143">Int32</span><span class="sxs-lookup"><span data-stu-id="22328-143">Int32</span></span>|<span data-ttu-id="22328-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22328-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="22328-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="22328-145">Response</span></span>
<span data-ttu-id="22328-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22328-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22328-147">Пример</span><span class="sxs-lookup"><span data-stu-id="22328-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="22328-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="22328-148">Request</span></span>
<span data-ttu-id="22328-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22328-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="22328-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="22328-150">Response</span></span>
<span data-ttu-id="22328-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22328-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



