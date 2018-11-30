---
title: Список importedWindowsAutopilotDeviceIdentityUploads
description: Свойства списка и связей объектов importedWindowsAutopilotDeviceIdentityUpload.
ms.openlocfilehash: 710bc72af1d674999c44b3608c7eec5cde0798b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080462"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="6284f-103">Список importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="6284f-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="6284f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6284f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6284f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6284f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6284f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6284f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6284f-107">Свойства списка и связей объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="6284f-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6284f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6284f-108">Prerequisites</span></span>
<span data-ttu-id="6284f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6284f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6284f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6284f-111">Permission type</span></span>|<span data-ttu-id="6284f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6284f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6284f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6284f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6284f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6284f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6284f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6284f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6284f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6284f-116">Not supported.</span></span>|
|<span data-ttu-id="6284f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6284f-117">Application</span></span>|<span data-ttu-id="6284f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6284f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6284f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6284f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="6284f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6284f-120">Request headers</span></span>
|<span data-ttu-id="6284f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6284f-121">Header</span></span>|<span data-ttu-id="6284f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6284f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6284f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6284f-123">Authorization</span></span>|<span data-ttu-id="6284f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6284f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6284f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6284f-125">Accept</span></span>|<span data-ttu-id="6284f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6284f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6284f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6284f-127">Request body</span></span>
<span data-ttu-id="6284f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6284f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6284f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6284f-129">Response</span></span>
<span data-ttu-id="6284f-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6284f-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6284f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6284f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6284f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6284f-132">Request</span></span>
<span data-ttu-id="6284f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6284f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="6284f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6284f-134">Response</span></span>
<span data-ttu-id="6284f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6284f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





