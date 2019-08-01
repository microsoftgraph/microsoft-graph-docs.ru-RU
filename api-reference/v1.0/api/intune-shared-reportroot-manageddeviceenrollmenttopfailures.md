---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfd5710a310bba3d794902eaf01027538819f1bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023365"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="ad1f8-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="ad1f8-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="ad1f8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad1f8-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad1f8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad1f8-106">Prerequisites</span></span>
<span data-ttu-id="ad1f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad1f8-109">Permission type</span></span>|<span data-ttu-id="ad1f8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad1f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad1f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad1f8-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ad1f8-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="ad1f8-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="ad1f8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1f8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad1f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad1f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad1f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-115">Not supported.</span></span>|
|<span data-ttu-id="ad1f8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad1f8-116">Application</span></span>|<span data-ttu-id="ad1f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad1f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad1f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="ad1f8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad1f8-119">Request headers</span></span>
|<span data-ttu-id="ad1f8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad1f8-120">Header</span></span>|<span data-ttu-id="ad1f8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad1f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad1f8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad1f8-122">Authorization</span></span>|<span data-ttu-id="ad1f8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad1f8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ad1f8-124">Accept</span></span>|<span data-ttu-id="ad1f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad1f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad1f8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad1f8-126">Request body</span></span>
<span data-ttu-id="ad1f8-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ad1f8-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ad1f8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad1f8-129">Property</span></span>|<span data-ttu-id="ad1f8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad1f8-130">Type</span></span>|<span data-ttu-id="ad1f8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad1f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad1f8-132">period</span><span class="sxs-lookup"><span data-stu-id="ad1f8-132">period</span></span>|<span data-ttu-id="ad1f8-133">String</span><span class="sxs-lookup"><span data-stu-id="ad1f8-133">String</span></span>|<span data-ttu-id="ad1f8-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ad1f8-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ad1f8-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad1f8-135">Response</span></span>
<span data-ttu-id="ad1f8-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad1f8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ad1f8-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad1f8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad1f8-138">Request</span></span>
<span data-ttu-id="ad1f8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ad1f8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad1f8-140">Response</span></span>
<span data-ttu-id="ad1f8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad1f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




