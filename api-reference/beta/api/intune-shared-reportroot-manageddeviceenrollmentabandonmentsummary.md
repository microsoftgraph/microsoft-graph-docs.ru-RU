---
title: Функция Манажеддевицеенроллментабандонментсуммари
description: Метаданные для сводного отчета об отмене регистрации
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0ac224ec30110abd39675c1fcb8c64e3087185a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458170"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="73a94-103">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="73a94-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

<span data-ttu-id="73a94-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="73a94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73a94-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73a94-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73a94-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73a94-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73a94-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73a94-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73a94-108">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="73a94-108">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73a94-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73a94-109">Prerequisites</span></span>
<span data-ttu-id="73a94-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73a94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73a94-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73a94-112">Permission type</span></span>|<span data-ttu-id="73a94-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73a94-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73a94-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73a94-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73a94-115">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="73a94-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="73a94-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73a94-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="73a94-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73a94-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73a94-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73a94-118">Not supported.</span></span>|
|<span data-ttu-id="73a94-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73a94-119">Application</span></span>||
| <span data-ttu-id="73a94-120">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="73a94-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="73a94-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73a94-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73a94-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73a94-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="73a94-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73a94-123">Request headers</span></span>
|<span data-ttu-id="73a94-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73a94-124">Header</span></span>|<span data-ttu-id="73a94-125">Значение</span><span class="sxs-lookup"><span data-stu-id="73a94-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73a94-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="73a94-126">Authorization</span></span>|<span data-ttu-id="73a94-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73a94-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73a94-128">Accept</span><span class="sxs-lookup"><span data-stu-id="73a94-128">Accept</span></span>|<span data-ttu-id="73a94-129">application/json</span><span class="sxs-lookup"><span data-stu-id="73a94-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73a94-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73a94-130">Request body</span></span>
<span data-ttu-id="73a94-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="73a94-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="73a94-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="73a94-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="73a94-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="73a94-133">Property</span></span>|<span data-ttu-id="73a94-134">Тип</span><span class="sxs-lookup"><span data-stu-id="73a94-134">Type</span></span>|<span data-ttu-id="73a94-135">Описание</span><span class="sxs-lookup"><span data-stu-id="73a94-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73a94-136">skip</span><span class="sxs-lookup"><span data-stu-id="73a94-136">skip</span></span>|<span data-ttu-id="73a94-137">Int32</span><span class="sxs-lookup"><span data-stu-id="73a94-137">Int32</span></span>|<span data-ttu-id="73a94-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73a94-138">Not yet documented</span></span>|
|<span data-ttu-id="73a94-139">top</span><span class="sxs-lookup"><span data-stu-id="73a94-139">top</span></span>|<span data-ttu-id="73a94-140">Int32</span><span class="sxs-lookup"><span data-stu-id="73a94-140">Int32</span></span>|<span data-ttu-id="73a94-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73a94-141">Not yet documented</span></span>|
|<span data-ttu-id="73a94-142">filter</span><span class="sxs-lookup"><span data-stu-id="73a94-142">filter</span></span>|<span data-ttu-id="73a94-143">String</span><span class="sxs-lookup"><span data-stu-id="73a94-143">String</span></span>|<span data-ttu-id="73a94-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73a94-144">Not yet documented</span></span>|
|<span data-ttu-id="73a94-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="73a94-145">skipToken</span></span>|<span data-ttu-id="73a94-146">String</span><span class="sxs-lookup"><span data-stu-id="73a94-146">String</span></span>|<span data-ttu-id="73a94-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73a94-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="73a94-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="73a94-148">Response</span></span>
<span data-ttu-id="73a94-149">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73a94-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73a94-150">Пример</span><span class="sxs-lookup"><span data-stu-id="73a94-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="73a94-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a94-151">Request</span></span>
<span data-ttu-id="73a94-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a94-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="73a94-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a94-153">Response</span></span>
<span data-ttu-id="73a94-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73a94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













