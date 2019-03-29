---
title: Получение Импортедвиндовсаутопилотдевицеидентитюплоад
description: Чтение свойств и связей объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cb9962e4b1328c75558c9ff77b6dabe2f86c4de
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958377"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="b9a4f-103">Получение Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="b9a4f-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="b9a4f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a4f-105">Чтение свойств и связей объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a4f-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9a4f-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9a4f-106">Prerequisites</span></span>
<span data-ttu-id="b9a4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a4f-109">Permission type</span></span>|<span data-ttu-id="b9a4f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9a4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9a4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9a4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9a4f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9a4f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b9a4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9a4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9a4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-114">Not supported.</span></span>|
|<span data-ttu-id="b9a4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9a4f-115">Application</span></span>|<span data-ttu-id="b9a4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9a4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9a4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9a4f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9a4f-118">Optional query parameters</span></span>
<span data-ttu-id="b9a4f-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9a4f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9a4f-120">Request headers</span></span>
|<span data-ttu-id="b9a4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9a4f-121">Header</span></span>|<span data-ttu-id="b9a4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9a4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9a4f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9a4f-123">Authorization</span></span>|<span data-ttu-id="b9a4f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9a4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9a4f-125">Accept</span></span>|<span data-ttu-id="b9a4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9a4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9a4f-127">Request body</span></span>
<span data-ttu-id="b9a4f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a4f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9a4f-129">Response</span></span>
<span data-ttu-id="b9a4f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a4f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9a4f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9a4f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9a4f-132">Request</span></span>
<span data-ttu-id="b9a4f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="b9a4f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a4f-134">Response</span></span>
<span data-ttu-id="b9a4f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9a4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



