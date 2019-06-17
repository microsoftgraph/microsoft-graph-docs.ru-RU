---
title: Действие wipe
description: Очистка устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b7c1c39104180e6edc82fc49b21d2df05687340
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958132"
---
# <a name="wipe-action"></a><span data-ttu-id="249a5-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="249a5-103">wipe action</span></span>

> <span data-ttu-id="249a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="249a5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="249a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="249a5-106">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="249a5-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="249a5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="249a5-107">Prerequisites</span></span>
<span data-ttu-id="249a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="249a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="249a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="249a5-110">Permission type</span></span>|<span data-ttu-id="249a5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="249a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="249a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="249a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="249a5-113">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="249a5-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="249a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="249a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="249a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249a5-115">Not supported.</span></span>|
|<span data-ttu-id="249a5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="249a5-116">Application</span></span>|<span data-ttu-id="249a5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="249a5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="249a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="249a5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="249a5-119">Request headers</span></span>
|<span data-ttu-id="249a5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="249a5-120">Header</span></span>|<span data-ttu-id="249a5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="249a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="249a5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="249a5-122">Authorization</span></span>|<span data-ttu-id="249a5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="249a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="249a5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="249a5-124">Accept</span></span>|<span data-ttu-id="249a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="249a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="249a5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="249a5-126">Request body</span></span>
<span data-ttu-id="249a5-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="249a5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="249a5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="249a5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="249a5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="249a5-129">Property</span></span>|<span data-ttu-id="249a5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="249a5-130">Type</span></span>|<span data-ttu-id="249a5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="249a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="249a5-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="249a5-132">keepEnrollmentData</span></span>|<span data-ttu-id="249a5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="249a5-133">Boolean</span></span>|<span data-ttu-id="249a5-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="249a5-134">Not yet documented</span></span>|
|<span data-ttu-id="249a5-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="249a5-135">keepUserData</span></span>|<span data-ttu-id="249a5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="249a5-136">Boolean</span></span>|<span data-ttu-id="249a5-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="249a5-137">Not yet documented</span></span>|
|<span data-ttu-id="249a5-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="249a5-138">macOsUnlockCode</span></span>|<span data-ttu-id="249a5-139">String</span><span class="sxs-lookup"><span data-stu-id="249a5-139">String</span></span>|<span data-ttu-id="249a5-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="249a5-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="249a5-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="249a5-141">Response</span></span>
<span data-ttu-id="249a5-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="249a5-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="249a5-143">Пример</span><span class="sxs-lookup"><span data-stu-id="249a5-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="249a5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="249a5-144">Request</span></span>
<span data-ttu-id="249a5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="249a5-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="249a5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="249a5-146">Response</span></span>
<span data-ttu-id="249a5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="249a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





