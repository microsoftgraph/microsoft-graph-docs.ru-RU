---
title: Действие wipe
description: Очистка устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6011accbde9a0670a2a780aeeea99b17e9c19237
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985113"
---
# <a name="wipe-action"></a><span data-ttu-id="0cd8d-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="0cd8d-103">wipe action</span></span>

<span data-ttu-id="0cd8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cd8d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd8d-106">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="0cd8d-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd8d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd8d-107">Prerequisites</span></span>
<span data-ttu-id="0cd8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd8d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd8d-110">Permission type</span></span>|<span data-ttu-id="0cd8d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd8d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd8d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd8d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd8d-113">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0cd8d-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0cd8d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd8d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-115">Not supported.</span></span>|
|<span data-ttu-id="0cd8d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cd8d-116">Application</span></span>|<span data-ttu-id="0cd8d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd8d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd8d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="0cd8d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0cd8d-119">Request headers</span></span>
|<span data-ttu-id="0cd8d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd8d-120">Header</span></span>|<span data-ttu-id="0cd8d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd8d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd8d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd8d-122">Authorization</span></span>|<span data-ttu-id="0cd8d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd8d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd8d-124">Accept</span></span>|<span data-ttu-id="0cd8d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd8d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd8d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0cd8d-126">Request body</span></span>
<span data-ttu-id="0cd8d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0cd8d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0cd8d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd8d-129">Property</span></span>|<span data-ttu-id="0cd8d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0cd8d-130">Type</span></span>|<span data-ttu-id="0cd8d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd8d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd8d-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="0cd8d-132">keepEnrollmentData</span></span>|<span data-ttu-id="0cd8d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cd8d-133">Boolean</span></span>|<span data-ttu-id="0cd8d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0cd8d-134">Not yet documented</span></span>|
|<span data-ttu-id="0cd8d-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="0cd8d-135">keepUserData</span></span>|<span data-ttu-id="0cd8d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cd8d-136">Boolean</span></span>|<span data-ttu-id="0cd8d-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0cd8d-137">Not yet documented</span></span>|
|<span data-ttu-id="0cd8d-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="0cd8d-138">macOsUnlockCode</span></span>|<span data-ttu-id="0cd8d-139">String</span><span class="sxs-lookup"><span data-stu-id="0cd8d-139">String</span></span>|<span data-ttu-id="0cd8d-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0cd8d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cd8d-141">Response</span></span>
<span data-ttu-id="0cd8d-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0cd8d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd8d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd8d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd8d-144">Request</span></span>
<span data-ttu-id="0cd8d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="0cd8d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd8d-146">Response</span></span>
<span data-ttu-id="0cd8d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









