---
title: функция managedDeviceEnrollmentTopFailures
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df7e3331194f274ea1b6035d640e780e212a88b0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732798"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="e926a-103">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="e926a-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="e926a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e926a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e926a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e926a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e926a-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e926a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e926a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e926a-107">Prerequisites</span></span>
<span data-ttu-id="e926a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e926a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e926a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e926a-110">Permission type</span></span>|<span data-ttu-id="e926a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e926a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e926a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e926a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e926a-113">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e926a-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e926a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e926a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e926a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e926a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e926a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e926a-116">Not supported.</span></span>|
|<span data-ttu-id="e926a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e926a-117">Application</span></span>|<span data-ttu-id="e926a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e926a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e926a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e926a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="e926a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e926a-120">Request headers</span></span>
|<span data-ttu-id="e926a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e926a-121">Header</span></span>|<span data-ttu-id="e926a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e926a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e926a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e926a-123">Authorization</span></span>|<span data-ttu-id="e926a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e926a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e926a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e926a-125">Accept</span></span>|<span data-ttu-id="e926a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e926a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e926a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e926a-127">Request body</span></span>
<span data-ttu-id="e926a-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e926a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e926a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="e926a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e926a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e926a-130">Property</span></span>|<span data-ttu-id="e926a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e926a-131">Type</span></span>|<span data-ttu-id="e926a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e926a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e926a-133">period</span><span class="sxs-lookup"><span data-stu-id="e926a-133">period</span></span>|<span data-ttu-id="e926a-134">String</span><span class="sxs-lookup"><span data-stu-id="e926a-134">String</span></span>|<span data-ttu-id="e926a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e926a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e926a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e926a-136">Response</span></span>
<span data-ttu-id="e926a-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e926a-137">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e926a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e926a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e926a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e926a-139">Request</span></span>
<span data-ttu-id="e926a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e926a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e926a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e926a-141">Response</span></span>
<span data-ttu-id="e926a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e926a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










