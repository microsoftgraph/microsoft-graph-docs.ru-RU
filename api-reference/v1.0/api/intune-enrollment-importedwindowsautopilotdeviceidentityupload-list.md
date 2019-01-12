---
title: Список importedWindowsAutopilotDeviceIdentityUploads
description: Свойства списка и связей объектов importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38c072ef398b3425fb114a1ec7c03918894168d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951287"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="9f707-103">Список importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="9f707-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="9f707-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f707-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f707-105">Свойства списка и связей объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="9f707-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f707-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f707-106">Prerequisites</span></span>
<span data-ttu-id="9f707-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f707-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f707-109">Permission type</span></span>|<span data-ttu-id="9f707-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f707-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f707-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f707-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f707-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f707-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9f707-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f707-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f707-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f707-114">Not supported.</span></span>|
|<span data-ttu-id="9f707-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f707-115">Application</span></span>|<span data-ttu-id="9f707-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f707-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f707-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f707-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="9f707-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f707-118">Request headers</span></span>
|<span data-ttu-id="9f707-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f707-119">Header</span></span>|<span data-ttu-id="9f707-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9f707-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f707-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f707-121">Authorization</span></span>|<span data-ttu-id="9f707-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f707-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f707-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9f707-123">Accept</span></span>|<span data-ttu-id="9f707-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f707-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f707-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f707-125">Request body</span></span>
<span data-ttu-id="9f707-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f707-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f707-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f707-127">Response</span></span>
<span data-ttu-id="9f707-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f707-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f707-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9f707-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f707-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f707-130">Request</span></span>
<span data-ttu-id="9f707-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f707-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="9f707-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f707-132">Response</span></span>
<span data-ttu-id="9f707-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f707-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```



