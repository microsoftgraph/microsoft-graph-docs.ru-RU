---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdc523507964f87863131ef114b102f383524a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576792"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="27bce-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="27bce-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="27bce-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27bce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27bce-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27bce-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27bce-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="27bce-106">Prerequisites</span></span>
<span data-ttu-id="27bce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27bce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27bce-109">Permission type</span></span>|<span data-ttu-id="27bce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27bce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27bce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27bce-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27bce-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="27bce-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="27bce-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27bce-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27bce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27bce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27bce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27bce-115">Not supported.</span></span>|
|<span data-ttu-id="27bce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27bce-116">Application</span></span>|<span data-ttu-id="27bce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27bce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27bce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27bce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="27bce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27bce-119">Request headers</span></span>
|<span data-ttu-id="27bce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27bce-120">Header</span></span>|<span data-ttu-id="27bce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="27bce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27bce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27bce-122">Authorization</span></span>|<span data-ttu-id="27bce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27bce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27bce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="27bce-124">Accept</span></span>|<span data-ttu-id="27bce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27bce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27bce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27bce-126">Request body</span></span>
<span data-ttu-id="27bce-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="27bce-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="27bce-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="27bce-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="27bce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="27bce-129">Property</span></span>|<span data-ttu-id="27bce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="27bce-130">Type</span></span>|<span data-ttu-id="27bce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="27bce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27bce-132">period</span><span class="sxs-lookup"><span data-stu-id="27bce-132">period</span></span>|<span data-ttu-id="27bce-133">String</span><span class="sxs-lookup"><span data-stu-id="27bce-133">String</span></span>|<span data-ttu-id="27bce-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="27bce-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27bce-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="27bce-135">Response</span></span>
<span data-ttu-id="27bce-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27bce-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27bce-137">Пример</span><span class="sxs-lookup"><span data-stu-id="27bce-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="27bce-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="27bce-138">Request</span></span>
<span data-ttu-id="27bce-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27bce-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="27bce-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="27bce-140">Response</span></span>
<span data-ttu-id="27bce-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27bce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




