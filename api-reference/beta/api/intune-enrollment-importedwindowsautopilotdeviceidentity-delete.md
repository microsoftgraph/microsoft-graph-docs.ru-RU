---
title: Удаление importedWindowsAutopilotDeviceIdentity
description: Удаляет importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d167701dc3c813386e05433c72a0a2e101fd0ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452590"
---
# <a name="delete-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="f4d55-103">Удаление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f4d55-103">Delete importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="f4d55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4d55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4d55-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4d55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4d55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4d55-107">Удаляет [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f4d55-107">Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4d55-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d55-108">Prerequisites</span></span>
<span data-ttu-id="f4d55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4d55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d55-111">Permission type</span></span>|<span data-ttu-id="f4d55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d55-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d55-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d55-116">Not supported.</span></span>|
|<span data-ttu-id="f4d55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d55-117">Application</span></span>|<span data-ttu-id="f4d55-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d55-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="f4d55-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4d55-120">Request headers</span></span>
|<span data-ttu-id="f4d55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4d55-121">Header</span></span>|<span data-ttu-id="f4d55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4d55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4d55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4d55-123">Authorization</span></span>|<span data-ttu-id="f4d55-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4d55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4d55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4d55-125">Accept</span></span>|<span data-ttu-id="f4d55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4d55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d55-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4d55-127">Request body</span></span>
<span data-ttu-id="f4d55-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4d55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4d55-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d55-129">Response</span></span>
<span data-ttu-id="f4d55-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4d55-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4d55-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4d55-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4d55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d55-132">Request</span></span>
<span data-ttu-id="f4d55-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d55-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="f4d55-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d55-134">Response</span></span>
<span data-ttu-id="f4d55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4d55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



