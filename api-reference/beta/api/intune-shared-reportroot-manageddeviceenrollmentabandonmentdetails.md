---
title: Функция Манажеддевицеенроллментабандонментдетаилс
description: Метаданные для отчета о прекращении регистрации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5721e0cb5e466ba684fa1e73572a1ecf87a398b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141064"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="f753e-103">Функция Манажеддевицеенроллментабандонментдетаилс</span><span class="sxs-lookup"><span data-stu-id="f753e-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="f753e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f753e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f753e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f753e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f753e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f753e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f753e-107">Метаданные для отчета о прекращении регистрации</span><span class="sxs-lookup"><span data-stu-id="f753e-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f753e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f753e-108">Prerequisites</span></span>
<span data-ttu-id="f753e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f753e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="f753e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f753e-111">Permission type</span></span>|<span data-ttu-id="f753e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f753e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f753e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f753e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f753e-114">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="f753e-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="f753e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f753e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f753e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f753e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f753e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f753e-117">Not supported.</span></span>|
|<span data-ttu-id="f753e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f753e-118">Application</span></span>|<span data-ttu-id="f753e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f753e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f753e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f753e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="f753e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f753e-121">Request headers</span></span>
|<span data-ttu-id="f753e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f753e-122">Header</span></span>|<span data-ttu-id="f753e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f753e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f753e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f753e-124">Authorization</span></span>|<span data-ttu-id="f753e-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f753e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f753e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f753e-126">Accept</span></span>|<span data-ttu-id="f753e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f753e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f753e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f753e-128">Request body</span></span>
<span data-ttu-id="f753e-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f753e-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f753e-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f753e-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f753e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f753e-131">Property</span></span>|<span data-ttu-id="f753e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f753e-132">Type</span></span>|<span data-ttu-id="f753e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f753e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f753e-134">skip</span><span class="sxs-lookup"><span data-stu-id="f753e-134">skip</span></span>|<span data-ttu-id="f753e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f753e-135">Int32</span></span>|<span data-ttu-id="f753e-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f753e-136">Not yet documented</span></span>|
|<span data-ttu-id="f753e-137">top</span><span class="sxs-lookup"><span data-stu-id="f753e-137">top</span></span>|<span data-ttu-id="f753e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f753e-138">Int32</span></span>|<span data-ttu-id="f753e-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f753e-139">Not yet documented</span></span>|
|<span data-ttu-id="f753e-140">filter</span><span class="sxs-lookup"><span data-stu-id="f753e-140">filter</span></span>|<span data-ttu-id="f753e-141">String</span><span class="sxs-lookup"><span data-stu-id="f753e-141">String</span></span>|<span data-ttu-id="f753e-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f753e-142">Not yet documented</span></span>|
|<span data-ttu-id="f753e-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="f753e-143">skipToken</span></span>|<span data-ttu-id="f753e-144">String</span><span class="sxs-lookup"><span data-stu-id="f753e-144">String</span></span>|<span data-ttu-id="f753e-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f753e-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f753e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f753e-146">Response</span></span>
<span data-ttu-id="f753e-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f753e-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f753e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f753e-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="f753e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f753e-149">Request</span></span>
<span data-ttu-id="f753e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f753e-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f753e-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="f753e-151">Response</span></span>
<span data-ttu-id="f753e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f753e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





