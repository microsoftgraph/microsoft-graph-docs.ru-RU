---
title: Действие recoverPasscode
description: Восстановление секретного кода
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1479fc585f460997d032315e0e6f9e71bcc0a23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513527"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="65e23-103">Действие recoverPasscode</span><span class="sxs-lookup"><span data-stu-id="65e23-103">recoverPasscode action</span></span>

<span data-ttu-id="65e23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65e23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65e23-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65e23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e23-106">Восстановление секретного кода</span><span class="sxs-lookup"><span data-stu-id="65e23-106">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65e23-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="65e23-107">Prerequisites</span></span>
<span data-ttu-id="65e23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65e23-110">Permission type</span></span>|<span data-ttu-id="65e23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65e23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65e23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65e23-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="65e23-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="65e23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65e23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e23-115">Not supported.</span></span>|
|<span data-ttu-id="65e23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65e23-116">Application</span></span>|<span data-ttu-id="65e23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65e23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="65e23-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65e23-119">Request headers</span></span>
|<span data-ttu-id="65e23-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65e23-120">Header</span></span>|<span data-ttu-id="65e23-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65e23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e23-122">Authorization</span></span>|<span data-ttu-id="65e23-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65e23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e23-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65e23-124">Accept</span></span>|<span data-ttu-id="65e23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65e23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e23-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65e23-126">Request body</span></span>
<span data-ttu-id="65e23-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65e23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65e23-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="65e23-128">Response</span></span>
<span data-ttu-id="65e23-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65e23-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65e23-130">Пример</span><span class="sxs-lookup"><span data-stu-id="65e23-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="65e23-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="65e23-131">Request</span></span>
<span data-ttu-id="65e23-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65e23-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="65e23-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="65e23-133">Response</span></span>
<span data-ttu-id="65e23-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65e23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




