---
title: Функция Манажеддевицеенроллментабандонментсуммари
description: Метаданные для сводного отчета об отмене регистрации
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62ed37262c8c9a2ed75df9b4e7c497c28bc61847
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800692"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="73256-103">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="73256-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="73256-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73256-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73256-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73256-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73256-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73256-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73256-107">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="73256-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73256-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73256-108">Prerequisites</span></span>
<span data-ttu-id="73256-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73256-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73256-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73256-111">Permission type</span></span>|<span data-ttu-id="73256-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73256-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73256-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73256-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73256-114">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="73256-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="73256-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73256-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="73256-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73256-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73256-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73256-117">Not supported.</span></span>|
|<span data-ttu-id="73256-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="73256-118">Application</span></span>||
| <span data-ttu-id="73256-119">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="73256-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="73256-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73256-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73256-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73256-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="73256-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73256-122">Request headers</span></span>
|<span data-ttu-id="73256-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73256-123">Header</span></span>|<span data-ttu-id="73256-124">Значение</span><span class="sxs-lookup"><span data-stu-id="73256-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73256-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73256-125">Authorization</span></span>|<span data-ttu-id="73256-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73256-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73256-127">Accept</span><span class="sxs-lookup"><span data-stu-id="73256-127">Accept</span></span>|<span data-ttu-id="73256-128">application/json</span><span class="sxs-lookup"><span data-stu-id="73256-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73256-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73256-129">Request body</span></span>
<span data-ttu-id="73256-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="73256-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="73256-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="73256-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="73256-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="73256-132">Property</span></span>|<span data-ttu-id="73256-133">Тип</span><span class="sxs-lookup"><span data-stu-id="73256-133">Type</span></span>|<span data-ttu-id="73256-134">Описание</span><span class="sxs-lookup"><span data-stu-id="73256-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73256-135">skip</span><span class="sxs-lookup"><span data-stu-id="73256-135">skip</span></span>|<span data-ttu-id="73256-136">Int32</span><span class="sxs-lookup"><span data-stu-id="73256-136">Int32</span></span>|<span data-ttu-id="73256-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73256-137">Not yet documented</span></span>|
|<span data-ttu-id="73256-138">top</span><span class="sxs-lookup"><span data-stu-id="73256-138">top</span></span>|<span data-ttu-id="73256-139">Int32</span><span class="sxs-lookup"><span data-stu-id="73256-139">Int32</span></span>|<span data-ttu-id="73256-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73256-140">Not yet documented</span></span>|
|<span data-ttu-id="73256-141">filter</span><span class="sxs-lookup"><span data-stu-id="73256-141">filter</span></span>|<span data-ttu-id="73256-142">String</span><span class="sxs-lookup"><span data-stu-id="73256-142">String</span></span>|<span data-ttu-id="73256-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73256-143">Not yet documented</span></span>|
|<span data-ttu-id="73256-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="73256-144">skipToken</span></span>|<span data-ttu-id="73256-145">String</span><span class="sxs-lookup"><span data-stu-id="73256-145">String</span></span>|<span data-ttu-id="73256-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="73256-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="73256-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="73256-147">Response</span></span>
<span data-ttu-id="73256-148">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73256-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73256-149">Пример</span><span class="sxs-lookup"><span data-stu-id="73256-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="73256-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="73256-150">Request</span></span>
<span data-ttu-id="73256-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73256-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="73256-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="73256-152">Response</span></span>
<span data-ttu-id="73256-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73256-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












