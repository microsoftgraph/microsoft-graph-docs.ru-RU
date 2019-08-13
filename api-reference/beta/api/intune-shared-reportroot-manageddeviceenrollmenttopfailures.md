---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4fb5496a36f40c6b9debbfcc46e0cc4938e7f8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350715"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="6440d-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="6440d-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="6440d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6440d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6440d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6440d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6440d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6440d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6440d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6440d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6440d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6440d-108">Prerequisites</span></span>
<span data-ttu-id="6440d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6440d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6440d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6440d-111">Permission type</span></span>|<span data-ttu-id="6440d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6440d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6440d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6440d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6440d-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="6440d-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6440d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6440d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6440d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6440d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6440d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6440d-117">Not supported.</span></span>|
|<span data-ttu-id="6440d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6440d-118">Application</span></span>|<span data-ttu-id="6440d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6440d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6440d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6440d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="6440d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6440d-121">Request headers</span></span>
|<span data-ttu-id="6440d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6440d-122">Header</span></span>|<span data-ttu-id="6440d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6440d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6440d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6440d-124">Authorization</span></span>|<span data-ttu-id="6440d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6440d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6440d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6440d-126">Accept</span></span>|<span data-ttu-id="6440d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6440d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6440d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6440d-128">Request body</span></span>
<span data-ttu-id="6440d-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6440d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6440d-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6440d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6440d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6440d-131">Property</span></span>|<span data-ttu-id="6440d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6440d-132">Type</span></span>|<span data-ttu-id="6440d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6440d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6440d-134">period</span><span class="sxs-lookup"><span data-stu-id="6440d-134">period</span></span>|<span data-ttu-id="6440d-135">String</span><span class="sxs-lookup"><span data-stu-id="6440d-135">String</span></span>|<span data-ttu-id="6440d-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6440d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6440d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6440d-137">Response</span></span>
<span data-ttu-id="6440d-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6440d-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6440d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6440d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6440d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6440d-140">Request</span></span>
<span data-ttu-id="6440d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6440d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6440d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6440d-142">Response</span></span>
<span data-ttu-id="6440d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6440d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






