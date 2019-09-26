---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cd1eed26f4bc9b29b0c8a7187869f0fded61e35
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195827"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="a82b1-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="a82b1-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="a82b1-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a82b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a82b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a82b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a82b1-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a82b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a82b1-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a82b1-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a82b1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a82b1-108">Prerequisites</span></span>
<span data-ttu-id="a82b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a82b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a82b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a82b1-111">Permission type</span></span>|<span data-ttu-id="a82b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a82b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a82b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a82b1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a82b1-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="a82b1-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a82b1-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82b1-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a82b1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a82b1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a82b1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a82b1-117">Not supported.</span></span>|
|<span data-ttu-id="a82b1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a82b1-118">Application</span></span>||
| <span data-ttu-id="a82b1-119">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="a82b1-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a82b1-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82b1-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a82b1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a82b1-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="a82b1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a82b1-122">Request headers</span></span>
|<span data-ttu-id="a82b1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a82b1-123">Header</span></span>|<span data-ttu-id="a82b1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a82b1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a82b1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a82b1-125">Authorization</span></span>|<span data-ttu-id="a82b1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a82b1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a82b1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a82b1-127">Accept</span></span>|<span data-ttu-id="a82b1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a82b1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a82b1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a82b1-129">Request body</span></span>
<span data-ttu-id="a82b1-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a82b1-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a82b1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a82b1-131">Property</span></span>|<span data-ttu-id="a82b1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a82b1-132">Type</span></span>|<span data-ttu-id="a82b1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a82b1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82b1-134">filter</span><span class="sxs-lookup"><span data-stu-id="a82b1-134">filter</span></span>|<span data-ttu-id="a82b1-135">String</span><span class="sxs-lookup"><span data-stu-id="a82b1-135">String</span></span>|<span data-ttu-id="a82b1-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a82b1-136">Not yet documented</span></span>|
|<span data-ttu-id="a82b1-137">skipToken</span><span class="sxs-lookup"><span data-stu-id="a82b1-137">skipToken</span></span>|<span data-ttu-id="a82b1-138">String</span><span class="sxs-lookup"><span data-stu-id="a82b1-138">String</span></span>|<span data-ttu-id="a82b1-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a82b1-139">Not yet documented</span></span>|
|<span data-ttu-id="a82b1-140">skip</span><span class="sxs-lookup"><span data-stu-id="a82b1-140">skip</span></span>|<span data-ttu-id="a82b1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a82b1-141">Int32</span></span>|<span data-ttu-id="a82b1-142">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a82b1-142">Not yet documented</span></span>|
|<span data-ttu-id="a82b1-143">top</span><span class="sxs-lookup"><span data-stu-id="a82b1-143">top</span></span>|<span data-ttu-id="a82b1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a82b1-144">Int32</span></span>|<span data-ttu-id="a82b1-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a82b1-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a82b1-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="a82b1-146">Response</span></span>
<span data-ttu-id="a82b1-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a82b1-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a82b1-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a82b1-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a82b1-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a82b1-149">Request</span></span>
<span data-ttu-id="a82b1-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a82b1-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a82b1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a82b1-151">Response</span></span>
<span data-ttu-id="a82b1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a82b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







