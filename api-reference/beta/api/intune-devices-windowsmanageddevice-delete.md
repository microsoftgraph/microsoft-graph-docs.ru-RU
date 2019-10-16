---
title: Удаление Виндовсманажеддевице
description: Удаляет объект Виндовсманажеддевице.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea55fc0896d8fe1ed69cc637479eb7f8fcfd2b73
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526801"
---
# <a name="delete-windowsmanageddevice"></a><span data-ttu-id="7a434-103">Удаление Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="7a434-103">Delete windowsManagedDevice</span></span>

> <span data-ttu-id="7a434-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a434-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a434-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a434-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a434-106">Удаляет объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="7a434-106">Deletes a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a434-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a434-107">Prerequisites</span></span>
<span data-ttu-id="7a434-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a434-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a434-110">Permission type</span></span>|<span data-ttu-id="7a434-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a434-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a434-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a434-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a434-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a434-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7a434-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a434-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a434-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a434-115">Not supported.</span></span>|
|<span data-ttu-id="7a434-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7a434-116">Application</span></span>|<span data-ttu-id="7a434-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a434-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a434-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a434-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="7a434-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a434-119">Request headers</span></span>
|<span data-ttu-id="7a434-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a434-120">Header</span></span>|<span data-ttu-id="7a434-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7a434-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a434-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a434-122">Authorization</span></span>|<span data-ttu-id="7a434-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a434-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a434-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7a434-124">Accept</span></span>|<span data-ttu-id="7a434-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a434-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a434-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a434-126">Request body</span></span>
<span data-ttu-id="7a434-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a434-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a434-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a434-128">Response</span></span>
<span data-ttu-id="7a434-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a434-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a434-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7a434-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a434-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a434-131">Request</span></span>
<span data-ttu-id="7a434-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a434-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="7a434-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a434-133">Response</span></span>
<span data-ttu-id="7a434-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a434-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






