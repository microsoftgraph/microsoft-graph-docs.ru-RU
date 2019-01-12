---
title: функция autopilotDeviceStream
description: Создание запроса загрузки с потоком автопилот устройство в нем.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 656a3c525ac1eb6ede3efaa0759e28f6c32c5972
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968457"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="95365-103">функция autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="95365-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="95365-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95365-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95365-105">Создание запроса загрузки с потоком автопилот устройство в нем.</span><span class="sxs-lookup"><span data-stu-id="95365-105">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95365-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95365-106">Prerequisites</span></span>
<span data-ttu-id="95365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95365-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95365-109">Permission type</span></span>|<span data-ttu-id="95365-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95365-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95365-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95365-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95365-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95365-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95365-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95365-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95365-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95365-114">Not supported.</span></span>|
|<span data-ttu-id="95365-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95365-115">Application</span></span>|<span data-ttu-id="95365-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95365-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95365-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95365-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="95365-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95365-118">Request headers</span></span>
|<span data-ttu-id="95365-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95365-119">Header</span></span>|<span data-ttu-id="95365-120">Значение</span><span class="sxs-lookup"><span data-stu-id="95365-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95365-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95365-121">Authorization</span></span>|<span data-ttu-id="95365-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="95365-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95365-123">Accept</span><span class="sxs-lookup"><span data-stu-id="95365-123">Accept</span></span>|<span data-ttu-id="95365-124">application/json</span><span class="sxs-lookup"><span data-stu-id="95365-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95365-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95365-125">Request body</span></span>
<span data-ttu-id="95365-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95365-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95365-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="95365-127">Response</span></span>
<span data-ttu-id="95365-128">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95365-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95365-129">Пример</span><span class="sxs-lookup"><span data-stu-id="95365-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="95365-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="95365-130">Request</span></span>
<span data-ttu-id="95365-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95365-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="95365-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="95365-132">Response</span></span>
<span data-ttu-id="95365-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="95365-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



