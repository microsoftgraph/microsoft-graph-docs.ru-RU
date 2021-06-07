---
title: Действие wipe
description: Очистка устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df60cbab44f622f4620514594202a60582a0cf76
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756150"
---
# <a name="wipe-action"></a><span data-ttu-id="a68e5-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="a68e5-103">wipe action</span></span>

<span data-ttu-id="a68e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a68e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a68e5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a68e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a68e5-106">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="a68e5-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a68e5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a68e5-107">Prerequisites</span></span>
<span data-ttu-id="a68e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a68e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a68e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a68e5-110">Permission type</span></span>|<span data-ttu-id="a68e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a68e5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a68e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a68e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a68e5-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a68e5-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a68e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a68e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a68e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68e5-115">Not supported.</span></span>|
|<span data-ttu-id="a68e5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a68e5-116">Application</span></span>|<span data-ttu-id="a68e5-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a68e5-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a68e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a68e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="a68e5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a68e5-119">Request headers</span></span>
|<span data-ttu-id="a68e5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a68e5-120">Header</span></span>|<span data-ttu-id="a68e5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a68e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a68e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a68e5-122">Authorization</span></span>|<span data-ttu-id="a68e5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a68e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a68e5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a68e5-124">Accept</span></span>|<span data-ttu-id="a68e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a68e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a68e5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a68e5-126">Request body</span></span>
<span data-ttu-id="a68e5-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a68e5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a68e5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a68e5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a68e5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a68e5-129">Property</span></span>|<span data-ttu-id="a68e5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a68e5-130">Type</span></span>|<span data-ttu-id="a68e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a68e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68e5-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="a68e5-132">keepEnrollmentData</span></span>|<span data-ttu-id="a68e5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a68e5-133">Boolean</span></span>|<span data-ttu-id="a68e5-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a68e5-134">Not yet documented</span></span>|
|<span data-ttu-id="a68e5-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="a68e5-135">keepUserData</span></span>|<span data-ttu-id="a68e5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="a68e5-136">Boolean</span></span>|<span data-ttu-id="a68e5-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a68e5-137">Not yet documented</span></span>|
|<span data-ttu-id="a68e5-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="a68e5-138">macOsUnlockCode</span></span>|<span data-ttu-id="a68e5-139">String</span><span class="sxs-lookup"><span data-stu-id="a68e5-139">String</span></span>|<span data-ttu-id="a68e5-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a68e5-140">Not yet documented</span></span>|
|<span data-ttu-id="a68e5-141">persistEsimDataPlan</span><span class="sxs-lookup"><span data-stu-id="a68e5-141">persistEsimDataPlan</span></span>|<span data-ttu-id="a68e5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="a68e5-142">Boolean</span></span>|<span data-ttu-id="a68e5-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a68e5-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a68e5-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="a68e5-144">Response</span></span>
<span data-ttu-id="a68e5-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a68e5-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a68e5-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a68e5-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a68e5-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a68e5-147">Request</span></span>
<span data-ttu-id="a68e5-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a68e5-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 141

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "persistEsimDataPlan": true
}
```

### <a name="response"></a><span data-ttu-id="a68e5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a68e5-149">Response</span></span>
<span data-ttu-id="a68e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a68e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




