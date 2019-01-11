---
title: Получение importedWindowsAutopilotDeviceIdentityUpload
description: Чтение свойства и связи объекта importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 369a1dadd706efc05db6029ab912e964f98bc620
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837039"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="ad22a-103">Получение importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="ad22a-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="ad22a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad22a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad22a-105">Чтение свойства и связи объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="ad22a-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad22a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad22a-106">Prerequisites</span></span>
<span data-ttu-id="ad22a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad22a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad22a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad22a-109">Permission type</span></span>|<span data-ttu-id="ad22a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad22a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad22a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad22a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad22a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad22a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ad22a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad22a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad22a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad22a-114">Not supported.</span></span>|
|<span data-ttu-id="ad22a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad22a-115">Application</span></span>|<span data-ttu-id="ad22a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad22a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad22a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad22a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad22a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad22a-118">Optional query parameters</span></span>
<span data-ttu-id="ad22a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad22a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad22a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad22a-120">Request headers</span></span>
|<span data-ttu-id="ad22a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad22a-121">Header</span></span>|<span data-ttu-id="ad22a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad22a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad22a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad22a-123">Authorization</span></span>|<span data-ttu-id="ad22a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad22a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad22a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad22a-125">Accept</span></span>|<span data-ttu-id="ad22a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad22a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad22a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad22a-127">Request body</span></span>
<span data-ttu-id="ad22a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad22a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad22a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad22a-129">Response</span></span>
<span data-ttu-id="ad22a-130">Успешно завершена, этот метод возвращает `200 OK` объект [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad22a-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad22a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad22a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad22a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad22a-132">Request</span></span>
<span data-ttu-id="ad22a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad22a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="ad22a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad22a-134">Response</span></span>
<span data-ttu-id="ad22a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad22a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
    "id": "8d639524-9524-8d63-2495-638d2495638d",
    "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
    "status": "pending"
  }
}
```



