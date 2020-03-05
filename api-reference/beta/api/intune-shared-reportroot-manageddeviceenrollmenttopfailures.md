---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c855e46f9beafc279018a59c3466d6f955507e17
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458156"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="88360-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="88360-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="88360-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="88360-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88360-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88360-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88360-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88360-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88360-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88360-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88360-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="88360-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88360-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="88360-109">Prerequisites</span></span>
<span data-ttu-id="88360-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88360-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88360-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88360-112">Permission type</span></span>|<span data-ttu-id="88360-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88360-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88360-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88360-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88360-115">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="88360-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88360-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88360-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88360-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88360-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88360-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88360-118">Not supported.</span></span>|
|<span data-ttu-id="88360-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88360-119">Application</span></span>||
| <span data-ttu-id="88360-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="88360-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88360-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88360-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88360-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88360-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="88360-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88360-123">Request headers</span></span>
|<span data-ttu-id="88360-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88360-124">Header</span></span>|<span data-ttu-id="88360-125">Значение</span><span class="sxs-lookup"><span data-stu-id="88360-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88360-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="88360-126">Authorization</span></span>|<span data-ttu-id="88360-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88360-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88360-128">Accept</span><span class="sxs-lookup"><span data-stu-id="88360-128">Accept</span></span>|<span data-ttu-id="88360-129">application/json</span><span class="sxs-lookup"><span data-stu-id="88360-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88360-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88360-130">Request body</span></span>
<span data-ttu-id="88360-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="88360-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="88360-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="88360-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="88360-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="88360-133">Property</span></span>|<span data-ttu-id="88360-134">Тип</span><span class="sxs-lookup"><span data-stu-id="88360-134">Type</span></span>|<span data-ttu-id="88360-135">Описание</span><span class="sxs-lookup"><span data-stu-id="88360-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88360-136">period</span><span class="sxs-lookup"><span data-stu-id="88360-136">period</span></span>|<span data-ttu-id="88360-137">String</span><span class="sxs-lookup"><span data-stu-id="88360-137">String</span></span>|<span data-ttu-id="88360-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="88360-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="88360-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="88360-139">Response</span></span>
<span data-ttu-id="88360-140">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88360-140">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88360-141">Пример</span><span class="sxs-lookup"><span data-stu-id="88360-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="88360-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="88360-142">Request</span></span>
<span data-ttu-id="88360-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88360-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="88360-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="88360-144">Response</span></span>
<span data-ttu-id="88360-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88360-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











