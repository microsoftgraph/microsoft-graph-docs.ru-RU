---
title: Действие locateDevice
description: Поиск устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26f3fd70bb9ffcd578e51425ba8a041c4a65566e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969858"
---
# <a name="locatedevice-action"></a><span data-ttu-id="6c357-103">Действие locateDevice</span><span class="sxs-lookup"><span data-stu-id="6c357-103">locateDevice action</span></span>

> <span data-ttu-id="6c357-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6c357-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c357-105">Поиск устройства</span><span class="sxs-lookup"><span data-stu-id="6c357-105">Locate a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c357-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6c357-106">Prerequisites</span></span>
<span data-ttu-id="6c357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c357-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c357-109">Permission type</span></span>|<span data-ttu-id="6c357-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c357-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c357-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c357-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c357-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6c357-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6c357-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c357-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c357-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c357-114">Not supported.</span></span>|
|<span data-ttu-id="6c357-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c357-115">Application</span></span>|<span data-ttu-id="6c357-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c357-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c357-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c357-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="6c357-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c357-118">Request headers</span></span>
|<span data-ttu-id="6c357-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c357-119">Header</span></span>|<span data-ttu-id="6c357-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6c357-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c357-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c357-121">Authorization</span></span>|<span data-ttu-id="6c357-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6c357-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c357-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6c357-123">Accept</span></span>|<span data-ttu-id="6c357-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c357-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c357-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c357-125">Request body</span></span>
<span data-ttu-id="6c357-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c357-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c357-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c357-127">Response</span></span>
<span data-ttu-id="6c357-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c357-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c357-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6c357-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c357-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c357-130">Request</span></span>
<span data-ttu-id="6c357-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c357-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="6c357-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c357-132">Response</span></span>
<span data-ttu-id="6c357-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6c357-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



