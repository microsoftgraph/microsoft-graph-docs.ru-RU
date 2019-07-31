---
title: Функция Манажеддевицеенроллментабандонментдетаилс
description: Метаданные для отчета о прекращении регистрации
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 618f5985a1d93a9cc45dc4ef93fe475853b7e959
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993552"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="58fae-103">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="58fae-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="58fae-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58fae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58fae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58fae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58fae-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58fae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58fae-107">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="58fae-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58fae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58fae-108">Prerequisites</span></span>
<span data-ttu-id="58fae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58fae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58fae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58fae-111">Permission type</span></span>|<span data-ttu-id="58fae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58fae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58fae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58fae-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="58fae-114">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="58fae-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="58fae-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58fae-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="58fae-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58fae-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58fae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58fae-117">Not supported.</span></span>|
|<span data-ttu-id="58fae-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58fae-118">Application</span></span>|<span data-ttu-id="58fae-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58fae-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58fae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58fae-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="58fae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58fae-121">Request headers</span></span>
|<span data-ttu-id="58fae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58fae-122">Header</span></span>|<span data-ttu-id="58fae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="58fae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58fae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58fae-124">Authorization</span></span>|<span data-ttu-id="58fae-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58fae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58fae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="58fae-126">Accept</span></span>|<span data-ttu-id="58fae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="58fae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58fae-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58fae-128">Request body</span></span>
<span data-ttu-id="58fae-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="58fae-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="58fae-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="58fae-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="58fae-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="58fae-131">Property</span></span>|<span data-ttu-id="58fae-132">Тип</span><span class="sxs-lookup"><span data-stu-id="58fae-132">Type</span></span>|<span data-ttu-id="58fae-133">Описание</span><span class="sxs-lookup"><span data-stu-id="58fae-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fae-134">skip</span><span class="sxs-lookup"><span data-stu-id="58fae-134">skip</span></span>|<span data-ttu-id="58fae-135">Int32</span><span class="sxs-lookup"><span data-stu-id="58fae-135">Int32</span></span>|<span data-ttu-id="58fae-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58fae-136">Not yet documented</span></span>|
|<span data-ttu-id="58fae-137">top</span><span class="sxs-lookup"><span data-stu-id="58fae-137">top</span></span>|<span data-ttu-id="58fae-138">Int32</span><span class="sxs-lookup"><span data-stu-id="58fae-138">Int32</span></span>|<span data-ttu-id="58fae-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58fae-139">Not yet documented</span></span>|
|<span data-ttu-id="58fae-140">filter</span><span class="sxs-lookup"><span data-stu-id="58fae-140">filter</span></span>|<span data-ttu-id="58fae-141">String</span><span class="sxs-lookup"><span data-stu-id="58fae-141">String</span></span>|<span data-ttu-id="58fae-142">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58fae-142">Not yet documented</span></span>|
|<span data-ttu-id="58fae-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="58fae-143">skipToken</span></span>|<span data-ttu-id="58fae-144">String</span><span class="sxs-lookup"><span data-stu-id="58fae-144">String</span></span>|<span data-ttu-id="58fae-145">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58fae-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58fae-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="58fae-146">Response</span></span>
<span data-ttu-id="58fae-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58fae-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58fae-148">Пример</span><span class="sxs-lookup"><span data-stu-id="58fae-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="58fae-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="58fae-149">Request</span></span>
<span data-ttu-id="58fae-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58fae-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="58fae-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="58fae-151">Response</span></span>
<span data-ttu-id="58fae-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58fae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





