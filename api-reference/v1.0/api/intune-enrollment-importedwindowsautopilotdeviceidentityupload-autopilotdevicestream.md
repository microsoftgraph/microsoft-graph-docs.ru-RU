---
title: функция autopilotDeviceStream
description: Создание запроса загрузки с потоком автопилот устройство в нем.
ms.openlocfilehash: 484b62f33a49ac73f3ba143d1936a8332888d431
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025607"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="ceaf6-103">функция autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="ceaf6-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="ceaf6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceaf6-105">Создание запроса загрузки с потоком автопилот устройство в нем.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-105">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceaf6-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ceaf6-106">Prerequisites</span></span>
<span data-ttu-id="ceaf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceaf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceaf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceaf6-109">Permission type</span></span>|<span data-ttu-id="ceaf6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceaf6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceaf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceaf6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ceaf6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceaf6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ceaf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceaf6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceaf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-114">Not supported.</span></span>|
|<span data-ttu-id="ceaf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceaf6-115">Application</span></span>|<span data-ttu-id="ceaf6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceaf6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceaf6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="ceaf6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceaf6-118">Request headers</span></span>
|<span data-ttu-id="ceaf6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ceaf6-119">Header</span></span>|<span data-ttu-id="ceaf6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ceaf6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceaf6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceaf6-121">Authorization</span></span>|<span data-ttu-id="ceaf6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ceaf6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceaf6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ceaf6-123">Accept</span></span>|<span data-ttu-id="ceaf6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ceaf6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceaf6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceaf6-125">Request body</span></span>
<span data-ttu-id="ceaf6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceaf6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ceaf6-127">Response</span></span>
<span data-ttu-id="ceaf6-128">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceaf6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ceaf6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceaf6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceaf6-130">Request</span></span>
<span data-ttu-id="ceaf6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ceaf6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="ceaf6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceaf6-132">Response</span></span>
<span data-ttu-id="ceaf6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ceaf6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



