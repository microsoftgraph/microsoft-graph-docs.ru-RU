---
title: функция managedDeviceEnrollmentFailureDetails
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08d9664ac74cd26018380844eebceabe42bb1154
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866995"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="05f6f-103">функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="05f6f-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="05f6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05f6f-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="05f6f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05f6f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f6f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05f6f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05f6f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05f6f-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05f6f-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05f6f-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05f6f-109">Prerequisites</span></span>
<span data-ttu-id="05f6f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05f6f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05f6f-112">Permission type</span></span>|<span data-ttu-id="05f6f-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05f6f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05f6f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05f6f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05f6f-115">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="05f6f-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="05f6f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f6f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05f6f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05f6f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05f6f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f6f-118">Not supported.</span></span>|
|<span data-ttu-id="05f6f-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="05f6f-119">Application</span></span>||
| <span data-ttu-id="05f6f-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="05f6f-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="05f6f-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f6f-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05f6f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05f6f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="05f6f-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05f6f-123">Request headers</span></span>
|<span data-ttu-id="05f6f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05f6f-124">Header</span></span>|<span data-ttu-id="05f6f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="05f6f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05f6f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05f6f-126">Authorization</span></span>|<span data-ttu-id="05f6f-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05f6f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05f6f-128">Accept</span><span class="sxs-lookup"><span data-stu-id="05f6f-128">Accept</span></span>|<span data-ttu-id="05f6f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="05f6f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05f6f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05f6f-130">Request body</span></span>
<span data-ttu-id="05f6f-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="05f6f-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="05f6f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="05f6f-132">Property</span></span>|<span data-ttu-id="05f6f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="05f6f-133">Type</span></span>|<span data-ttu-id="05f6f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="05f6f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05f6f-135">filter</span><span class="sxs-lookup"><span data-stu-id="05f6f-135">filter</span></span>|<span data-ttu-id="05f6f-136">String</span><span class="sxs-lookup"><span data-stu-id="05f6f-136">String</span></span>|<span data-ttu-id="05f6f-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05f6f-137">Not yet documented</span></span>|
|<span data-ttu-id="05f6f-138">skipToken</span><span class="sxs-lookup"><span data-stu-id="05f6f-138">skipToken</span></span>|<span data-ttu-id="05f6f-139">String</span><span class="sxs-lookup"><span data-stu-id="05f6f-139">String</span></span>|<span data-ttu-id="05f6f-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05f6f-140">Not yet documented</span></span>|
|<span data-ttu-id="05f6f-141">skip</span><span class="sxs-lookup"><span data-stu-id="05f6f-141">skip</span></span>|<span data-ttu-id="05f6f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="05f6f-142">Int32</span></span>|<span data-ttu-id="05f6f-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05f6f-143">Not yet documented</span></span>|
|<span data-ttu-id="05f6f-144">top</span><span class="sxs-lookup"><span data-stu-id="05f6f-144">top</span></span>|<span data-ttu-id="05f6f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="05f6f-145">Int32</span></span>|<span data-ttu-id="05f6f-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05f6f-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05f6f-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="05f6f-147">Response</span></span>
<span data-ttu-id="05f6f-148">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05f6f-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05f6f-149">Пример</span><span class="sxs-lookup"><span data-stu-id="05f6f-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="05f6f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="05f6f-150">Request</span></span>
<span data-ttu-id="05f6f-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05f6f-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="05f6f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f6f-152">Response</span></span>
<span data-ttu-id="05f6f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05f6f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










