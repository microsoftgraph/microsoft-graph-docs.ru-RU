---
title: Функция Манажеддевицеенроллментабандонментсуммари
description: Метаданные для сводного отчета об отмене регистрации
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7792bd9aef146b3b12b005510e2a955d072c802f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195834"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="b4cf8-103">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="b4cf8-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="b4cf8-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4cf8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4cf8-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4cf8-107">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="b4cf8-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4cf8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4cf8-108">Prerequisites</span></span>
<span data-ttu-id="b4cf8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4cf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4cf8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4cf8-111">Permission type</span></span>|<span data-ttu-id="b4cf8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4cf8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4cf8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4cf8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b4cf8-114">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="b4cf8-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b4cf8-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4cf8-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b4cf8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4cf8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4cf8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-117">Not supported.</span></span>|
|<span data-ttu-id="b4cf8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4cf8-118">Application</span></span>||
| <span data-ttu-id="b4cf8-119">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="b4cf8-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b4cf8-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4cf8-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4cf8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4cf8-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="b4cf8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4cf8-122">Request headers</span></span>
|<span data-ttu-id="b4cf8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4cf8-123">Header</span></span>|<span data-ttu-id="b4cf8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b4cf8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4cf8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4cf8-125">Authorization</span></span>|<span data-ttu-id="b4cf8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4cf8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b4cf8-127">Accept</span></span>|<span data-ttu-id="b4cf8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4cf8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4cf8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4cf8-129">Request body</span></span>
<span data-ttu-id="b4cf8-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b4cf8-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b4cf8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4cf8-132">Property</span></span>|<span data-ttu-id="b4cf8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b4cf8-133">Type</span></span>|<span data-ttu-id="b4cf8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cf8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4cf8-135">skip</span><span class="sxs-lookup"><span data-stu-id="b4cf8-135">skip</span></span>|<span data-ttu-id="b4cf8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b4cf8-136">Int32</span></span>|<span data-ttu-id="b4cf8-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-137">Not yet documented</span></span>|
|<span data-ttu-id="b4cf8-138">top</span><span class="sxs-lookup"><span data-stu-id="b4cf8-138">top</span></span>|<span data-ttu-id="b4cf8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b4cf8-139">Int32</span></span>|<span data-ttu-id="b4cf8-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-140">Not yet documented</span></span>|
|<span data-ttu-id="b4cf8-141">filter</span><span class="sxs-lookup"><span data-stu-id="b4cf8-141">filter</span></span>|<span data-ttu-id="b4cf8-142">String</span><span class="sxs-lookup"><span data-stu-id="b4cf8-142">String</span></span>|<span data-ttu-id="b4cf8-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-143">Not yet documented</span></span>|
|<span data-ttu-id="b4cf8-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="b4cf8-144">skipToken</span></span>|<span data-ttu-id="b4cf8-145">String</span><span class="sxs-lookup"><span data-stu-id="b4cf8-145">String</span></span>|<span data-ttu-id="b4cf8-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4cf8-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4cf8-147">Response</span></span>
<span data-ttu-id="b4cf8-148">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4cf8-149">Пример</span><span class="sxs-lookup"><span data-stu-id="b4cf8-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4cf8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4cf8-150">Request</span></span>
<span data-ttu-id="b4cf8-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b4cf8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4cf8-152">Response</span></span>
<span data-ttu-id="b4cf8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4cf8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









