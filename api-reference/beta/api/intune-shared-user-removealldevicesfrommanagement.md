---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9551cbe3c2cf1be162918feaaa52934bd9e1aac5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458009"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="69f62-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="69f62-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="69f62-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69f62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69f62-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="69f62-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69f62-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f62-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69f62-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f62-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f62-108">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="69f62-108">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69f62-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69f62-109">Prerequisites</span></span>
<span data-ttu-id="69f62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f62-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f62-112">Permission type</span></span>|<span data-ttu-id="69f62-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f62-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f62-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f62-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="69f62-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="69f62-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="69f62-116">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="69f62-116">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="69f62-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f62-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f62-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f62-118">Not supported.</span></span>|
|<span data-ttu-id="69f62-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f62-119">Application</span></span>||
| <span data-ttu-id="69f62-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="69f62-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="69f62-121">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="69f62-121">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f62-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f62-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="69f62-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69f62-123">Request headers</span></span>
|<span data-ttu-id="69f62-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f62-124">Header</span></span>|<span data-ttu-id="69f62-125">Значение</span><span class="sxs-lookup"><span data-stu-id="69f62-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f62-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f62-126">Authorization</span></span>|<span data-ttu-id="69f62-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f62-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f62-128">Accept</span><span class="sxs-lookup"><span data-stu-id="69f62-128">Accept</span></span>|<span data-ttu-id="69f62-129">application/json</span><span class="sxs-lookup"><span data-stu-id="69f62-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f62-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69f62-130">Request body</span></span>
<span data-ttu-id="69f62-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69f62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f62-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="69f62-132">Response</span></span>
<span data-ttu-id="69f62-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69f62-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="69f62-134">Пример</span><span class="sxs-lookup"><span data-stu-id="69f62-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="69f62-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f62-135">Request</span></span>
<span data-ttu-id="69f62-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f62-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="69f62-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f62-137">Response</span></span>
<span data-ttu-id="69f62-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













