---
title: Получение Импортедвиндовсаутопилотдевицеидентитюплоад
description: Чтение свойств и связей объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d376fe6ab41c3c8702b20a5cd9cb0cff7893250
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462898"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="ee0d2-103">Получение Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="ee0d2-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

<span data-ttu-id="ee0d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee0d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee0d2-106">Чтение свойств и связей объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="ee0d2-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee0d2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee0d2-107">Prerequisites</span></span>
<span data-ttu-id="ee0d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0d2-110">Permission type</span></span>|<span data-ttu-id="ee0d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee0d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee0d2-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee0d2-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ee0d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee0d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee0d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-115">Not supported.</span></span>|
|<span data-ttu-id="ee0d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee0d2-116">Application</span></span>|<span data-ttu-id="ee0d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee0d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee0d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee0d2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee0d2-119">Optional query parameters</span></span>
<span data-ttu-id="ee0d2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee0d2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee0d2-121">Request headers</span></span>
|<span data-ttu-id="ee0d2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee0d2-122">Header</span></span>|<span data-ttu-id="ee0d2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ee0d2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee0d2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee0d2-124">Authorization</span></span>|<span data-ttu-id="ee0d2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee0d2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ee0d2-126">Accept</span></span>|<span data-ttu-id="ee0d2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee0d2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0d2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee0d2-128">Request body</span></span>
<span data-ttu-id="ee0d2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee0d2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee0d2-130">Response</span></span>
<span data-ttu-id="ee0d2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee0d2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ee0d2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee0d2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee0d2-133">Request</span></span>
<span data-ttu-id="ee0d2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="ee0d2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0d2-135">Response</span></span>
<span data-ttu-id="ee0d2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee0d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






