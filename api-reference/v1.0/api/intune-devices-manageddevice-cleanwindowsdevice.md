---
title: Действие cleanWindowsDevice
description: Очистка устройства с Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cc8385c7394cdaa26decd89b53020161858e800
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083318"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="9fc79-103">Действие cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="9fc79-103">cleanWindowsDevice action</span></span>

<span data-ttu-id="9fc79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fc79-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fc79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fc79-106">Очистка устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="9fc79-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fc79-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9fc79-107">Prerequisites</span></span>
<span data-ttu-id="9fc79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc79-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc79-110">Permission type</span></span>|<span data-ttu-id="9fc79-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fc79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fc79-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fc79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fc79-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9fc79-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9fc79-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fc79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fc79-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fc79-115">Not supported.</span></span>|
|<span data-ttu-id="9fc79-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fc79-116">Application</span></span>|<span data-ttu-id="9fc79-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fc79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fc79-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fc79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="9fc79-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fc79-119">Request headers</span></span>
|<span data-ttu-id="9fc79-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fc79-120">Header</span></span>|<span data-ttu-id="9fc79-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9fc79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fc79-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fc79-122">Authorization</span></span>|<span data-ttu-id="9fc79-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fc79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fc79-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9fc79-124">Accept</span></span>|<span data-ttu-id="9fc79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fc79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fc79-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fc79-126">Request body</span></span>
<span data-ttu-id="9fc79-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fc79-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9fc79-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9fc79-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9fc79-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fc79-129">Property</span></span>|<span data-ttu-id="9fc79-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc79-130">Type</span></span>|<span data-ttu-id="9fc79-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc79-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="9fc79-132">keepUserData</span></span>|<span data-ttu-id="9fc79-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fc79-133">Boolean</span></span>|<span data-ttu-id="9fc79-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9fc79-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9fc79-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fc79-135">Response</span></span>
<span data-ttu-id="9fc79-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9fc79-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9fc79-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9fc79-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fc79-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc79-138">Request</span></span>
<span data-ttu-id="9fc79-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc79-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="9fc79-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc79-140">Response</span></span>
<span data-ttu-id="9fc79-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fc79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









