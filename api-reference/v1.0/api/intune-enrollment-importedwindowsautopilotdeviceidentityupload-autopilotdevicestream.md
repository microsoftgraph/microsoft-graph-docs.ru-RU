---
title: Функция Аутопилотдевицестреам
description: Создайте запрос на отправку с потоком устройства с автопилотом.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5499750978a8679753f0a1a168bee43684024a08
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471379"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="4831e-103">Функция Аутопилотдевицестреам</span><span class="sxs-lookup"><span data-stu-id="4831e-103">autopilotDeviceStream function</span></span>

<span data-ttu-id="4831e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4831e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4831e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4831e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4831e-106">Создайте запрос на отправку с потоком устройства с автопилотом.</span><span class="sxs-lookup"><span data-stu-id="4831e-106">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4831e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4831e-107">Prerequisites</span></span>
<span data-ttu-id="4831e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4831e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4831e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4831e-110">Permission type</span></span>|<span data-ttu-id="4831e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4831e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4831e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4831e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4831e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4831e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4831e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4831e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4831e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4831e-115">Not supported.</span></span>|
|<span data-ttu-id="4831e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4831e-116">Application</span></span>|<span data-ttu-id="4831e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4831e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4831e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4831e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="4831e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4831e-119">Request headers</span></span>
|<span data-ttu-id="4831e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4831e-120">Header</span></span>|<span data-ttu-id="4831e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4831e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4831e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4831e-122">Authorization</span></span>|<span data-ttu-id="4831e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4831e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4831e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4831e-124">Accept</span></span>|<span data-ttu-id="4831e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4831e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4831e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4831e-126">Request body</span></span>
<span data-ttu-id="4831e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4831e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4831e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4831e-128">Response</span></span>
<span data-ttu-id="4831e-129">В случае успеха эта функция возвращает код `200 OK` отклика и строку в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4831e-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4831e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4831e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4831e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4831e-131">Request</span></span>
<span data-ttu-id="4831e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4831e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="4831e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4831e-133">Response</span></span>
<span data-ttu-id="4831e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4831e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```






