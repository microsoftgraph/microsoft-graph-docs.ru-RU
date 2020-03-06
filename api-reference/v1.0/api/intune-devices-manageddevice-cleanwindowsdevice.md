---
title: Действие cleanWindowsDevice
description: Очистка устройства с Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd9018088ef84c9d6cb160ba9a22d41756393344
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513597"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="01a88-103">Действие cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="01a88-103">cleanWindowsDevice action</span></span>

<span data-ttu-id="01a88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01a88-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01a88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01a88-106">Очистка устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="01a88-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01a88-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01a88-107">Prerequisites</span></span>
<span data-ttu-id="01a88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a88-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01a88-110">Permission type</span></span>|<span data-ttu-id="01a88-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01a88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a88-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01a88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01a88-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="01a88-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="01a88-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01a88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a88-115">Not supported.</span></span>|
|<span data-ttu-id="01a88-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01a88-116">Application</span></span>|<span data-ttu-id="01a88-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a88-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01a88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="01a88-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01a88-119">Request headers</span></span>
|<span data-ttu-id="01a88-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01a88-120">Header</span></span>|<span data-ttu-id="01a88-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01a88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01a88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a88-122">Authorization</span></span>|<span data-ttu-id="01a88-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01a88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01a88-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01a88-124">Accept</span></span>|<span data-ttu-id="01a88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01a88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a88-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01a88-126">Request body</span></span>
<span data-ttu-id="01a88-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a88-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="01a88-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="01a88-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="01a88-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a88-129">Property</span></span>|<span data-ttu-id="01a88-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01a88-130">Type</span></span>|<span data-ttu-id="01a88-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01a88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01a88-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="01a88-132">keepUserData</span></span>|<span data-ttu-id="01a88-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="01a88-133">Boolean</span></span>|<span data-ttu-id="01a88-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="01a88-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="01a88-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="01a88-135">Response</span></span>
<span data-ttu-id="01a88-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01a88-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01a88-137">Пример</span><span class="sxs-lookup"><span data-stu-id="01a88-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="01a88-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="01a88-138">Request</span></span>
<span data-ttu-id="01a88-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01a88-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="01a88-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="01a88-140">Response</span></span>
<span data-ttu-id="01a88-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01a88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




