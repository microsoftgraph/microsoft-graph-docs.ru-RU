---
title: Действие updateWindowsDeviceAccount
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b189793dfb9351de9015b3052a88ac53e31fa85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829626"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="910ec-103">Действие updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="910ec-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="910ec-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="910ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="910ec-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="910ec-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="910ec-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="910ec-106">Prerequisites</span></span>
<span data-ttu-id="910ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="910ec-109">Permission type</span></span>|<span data-ttu-id="910ec-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="910ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="910ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="910ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="910ec-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="910ec-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="910ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="910ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="910ec-114">Not supported.</span></span>|
|<span data-ttu-id="910ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="910ec-115">Application</span></span>|<span data-ttu-id="910ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="910ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="910ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="910ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="910ec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="910ec-118">Request headers</span></span>
|<span data-ttu-id="910ec-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="910ec-119">Header</span></span>|<span data-ttu-id="910ec-120">Значение</span><span class="sxs-lookup"><span data-stu-id="910ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="910ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="910ec-121">Authorization</span></span>|<span data-ttu-id="910ec-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="910ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="910ec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="910ec-123">Accept</span></span>|<span data-ttu-id="910ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="910ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="910ec-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="910ec-125">Request body</span></span>
<span data-ttu-id="910ec-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="910ec-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="910ec-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="910ec-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="910ec-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="910ec-128">Property</span></span>|<span data-ttu-id="910ec-129">Тип</span><span class="sxs-lookup"><span data-stu-id="910ec-129">Type</span></span>|<span data-ttu-id="910ec-130">Описание</span><span class="sxs-lookup"><span data-stu-id="910ec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="910ec-131">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="910ec-131">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="910ec-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="910ec-132">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="910ec-133">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="910ec-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="910ec-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="910ec-134">Response</span></span>
<span data-ttu-id="910ec-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="910ec-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="910ec-136">Пример</span><span class="sxs-lookup"><span data-stu-id="910ec-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="910ec-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="910ec-137">Request</span></span>
<span data-ttu-id="910ec-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="910ec-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="910ec-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="910ec-139">Response</span></span>
<span data-ttu-id="910ec-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="910ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



