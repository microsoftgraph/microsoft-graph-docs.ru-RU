---
title: Функция Манажеддевицеенроллментабандонментдетаилс
description: Метаданные для отчета о прекращении регистрации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8d11c01ca9bee9c895947d4966b59f4690353f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408459"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="a1a32-103">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="a1a32-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

<span data-ttu-id="a1a32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1a32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1a32-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1a32-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1a32-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1a32-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1a32-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1a32-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1a32-108">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="a1a32-108">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1a32-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1a32-109">Prerequisites</span></span>
<span data-ttu-id="a1a32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a32-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1a32-112">Permission type</span></span>|<span data-ttu-id="a1a32-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1a32-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1a32-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1a32-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1a32-115">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="a1a32-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="a1a32-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a32-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a1a32-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1a32-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1a32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1a32-118">Not supported.</span></span>|
|<span data-ttu-id="a1a32-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="a1a32-119">Application</span></span>||
| <span data-ttu-id="a1a32-120">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="a1a32-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="a1a32-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a32-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1a32-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1a32-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="a1a32-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1a32-123">Request headers</span></span>
|<span data-ttu-id="a1a32-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1a32-124">Header</span></span>|<span data-ttu-id="a1a32-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a1a32-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1a32-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1a32-126">Authorization</span></span>|<span data-ttu-id="a1a32-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1a32-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1a32-128">Accept</span><span class="sxs-lookup"><span data-stu-id="a1a32-128">Accept</span></span>|<span data-ttu-id="a1a32-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a32-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a32-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1a32-130">Request body</span></span>
<span data-ttu-id="a1a32-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a1a32-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a1a32-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a1a32-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a1a32-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1a32-133">Property</span></span>|<span data-ttu-id="a1a32-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a1a32-134">Type</span></span>|<span data-ttu-id="a1a32-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a1a32-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1a32-136">skip</span><span class="sxs-lookup"><span data-stu-id="a1a32-136">skip</span></span>|<span data-ttu-id="a1a32-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a1a32-137">Int32</span></span>|<span data-ttu-id="a1a32-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a1a32-138">Not yet documented</span></span>|
|<span data-ttu-id="a1a32-139">top</span><span class="sxs-lookup"><span data-stu-id="a1a32-139">top</span></span>|<span data-ttu-id="a1a32-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a1a32-140">Int32</span></span>|<span data-ttu-id="a1a32-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a1a32-141">Not yet documented</span></span>|
|<span data-ttu-id="a1a32-142">filter</span><span class="sxs-lookup"><span data-stu-id="a1a32-142">filter</span></span>|<span data-ttu-id="a1a32-143">String</span><span class="sxs-lookup"><span data-stu-id="a1a32-143">String</span></span>|<span data-ttu-id="a1a32-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a1a32-144">Not yet documented</span></span>|
|<span data-ttu-id="a1a32-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="a1a32-145">skipToken</span></span>|<span data-ttu-id="a1a32-146">String</span><span class="sxs-lookup"><span data-stu-id="a1a32-146">String</span></span>|<span data-ttu-id="a1a32-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a1a32-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1a32-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1a32-148">Response</span></span>
<span data-ttu-id="a1a32-149">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1a32-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a32-150">Пример</span><span class="sxs-lookup"><span data-stu-id="a1a32-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1a32-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1a32-151">Request</span></span>
<span data-ttu-id="a1a32-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1a32-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a1a32-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1a32-153">Response</span></span>
<span data-ttu-id="a1a32-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1a32-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











