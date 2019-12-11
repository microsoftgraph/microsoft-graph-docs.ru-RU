---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3768a6386c9627acdc5653b7b91711ed21894a8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944696"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="7f3ad-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="7f3ad-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="7f3ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f3ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f3ad-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f3ad-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f3ad-107">Prerequisites</span></span>
<span data-ttu-id="7f3ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f3ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f3ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f3ad-110">Permission type</span></span>|<span data-ttu-id="7f3ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f3ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f3ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f3ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f3ad-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f3ad-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f3ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f3ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f3ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-115">Not supported.</span></span>|
|<span data-ttu-id="7f3ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f3ad-116">Application</span></span>|<span data-ttu-id="7f3ad-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f3ad-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f3ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f3ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="7f3ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f3ad-119">Request headers</span></span>
|<span data-ttu-id="7f3ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f3ad-120">Header</span></span>|<span data-ttu-id="7f3ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f3ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f3ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f3ad-122">Authorization</span></span>|<span data-ttu-id="7f3ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f3ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f3ad-124">Accept</span></span>|<span data-ttu-id="7f3ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f3ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f3ad-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f3ad-126">Request body</span></span>
<span data-ttu-id="7f3ad-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7f3ad-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7f3ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f3ad-129">Property</span></span>|<span data-ttu-id="7f3ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f3ad-130">Type</span></span>|<span data-ttu-id="7f3ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f3ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f3ad-132">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="7f3ad-132">notificationTitle</span></span>|<span data-ttu-id="7f3ad-133">String</span><span class="sxs-lookup"><span data-stu-id="7f3ad-133">String</span></span>|<span data-ttu-id="7f3ad-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-134">Not yet documented</span></span>|
|<span data-ttu-id="7f3ad-135">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="7f3ad-135">notificationBody</span></span>|<span data-ttu-id="7f3ad-136">String</span><span class="sxs-lookup"><span data-stu-id="7f3ad-136">String</span></span>|<span data-ttu-id="7f3ad-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7f3ad-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7f3ad-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f3ad-138">Response</span></span>
<span data-ttu-id="7f3ad-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f3ad-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7f3ad-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f3ad-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f3ad-141">Request</span></span>
<span data-ttu-id="7f3ad-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="7f3ad-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f3ad-143">Response</span></span>
<span data-ttu-id="7f3ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f3ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





