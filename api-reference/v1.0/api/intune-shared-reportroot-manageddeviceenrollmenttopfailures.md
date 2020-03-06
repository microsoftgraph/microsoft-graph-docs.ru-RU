---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bdcf397b9b4d7686219e99cab2a41bab02f3c5d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512022"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="14b77-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="14b77-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="14b77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14b77-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14b77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b77-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="14b77-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14b77-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14b77-107">Prerequisites</span></span>
<span data-ttu-id="14b77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14b77-110">Permission type</span></span>|<span data-ttu-id="14b77-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14b77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14b77-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="14b77-113">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="14b77-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="14b77-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b77-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14b77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14b77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b77-116">Not supported.</span></span>|
|<span data-ttu-id="14b77-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14b77-117">Application</span></span>|<span data-ttu-id="14b77-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14b77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="14b77-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14b77-120">Request headers</span></span>
|<span data-ttu-id="14b77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14b77-121">Header</span></span>|<span data-ttu-id="14b77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14b77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b77-123">Authorization</span></span>|<span data-ttu-id="14b77-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14b77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14b77-125">Accept</span></span>|<span data-ttu-id="14b77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14b77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14b77-127">Request body</span></span>
<span data-ttu-id="14b77-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="14b77-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="14b77-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="14b77-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="14b77-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14b77-130">Property</span></span>|<span data-ttu-id="14b77-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14b77-131">Type</span></span>|<span data-ttu-id="14b77-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14b77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b77-133">period</span><span class="sxs-lookup"><span data-stu-id="14b77-133">period</span></span>|<span data-ttu-id="14b77-134">String</span><span class="sxs-lookup"><span data-stu-id="14b77-134">String</span></span>|<span data-ttu-id="14b77-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="14b77-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14b77-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="14b77-136">Response</span></span>
<span data-ttu-id="14b77-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14b77-137">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b77-138">Пример</span><span class="sxs-lookup"><span data-stu-id="14b77-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="14b77-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="14b77-139">Request</span></span>
<span data-ttu-id="14b77-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14b77-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="14b77-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b77-141">Response</span></span>
<span data-ttu-id="14b77-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14b77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





