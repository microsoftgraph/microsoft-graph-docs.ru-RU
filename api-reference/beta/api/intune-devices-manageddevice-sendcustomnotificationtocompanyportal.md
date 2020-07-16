---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ca43e7c3fa83fea07b78fd0d9048c914eb7267d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792193"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="06326-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="06326-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="06326-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06326-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06326-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06326-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06326-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06326-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06326-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06326-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06326-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06326-108">Prerequisites</span></span>
<span data-ttu-id="06326-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06326-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06326-111">Permission type</span></span>|<span data-ttu-id="06326-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06326-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06326-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06326-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06326-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06326-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06326-116">Not supported.</span></span>|
|<span data-ttu-id="06326-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06326-117">Application</span></span>|<span data-ttu-id="06326-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06326-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06326-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/comanagedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="06326-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06326-120">Request headers</span></span>
|<span data-ttu-id="06326-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06326-121">Header</span></span>|<span data-ttu-id="06326-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06326-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06326-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06326-123">Authorization</span></span>|<span data-ttu-id="06326-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06326-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06326-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06326-125">Accept</span></span>|<span data-ttu-id="06326-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06326-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06326-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06326-127">Request body</span></span>
<span data-ttu-id="06326-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06326-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="06326-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="06326-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="06326-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06326-130">Property</span></span>|<span data-ttu-id="06326-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06326-131">Type</span></span>|<span data-ttu-id="06326-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06326-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06326-133">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="06326-133">notificationTitle</span></span>|<span data-ttu-id="06326-134">String</span><span class="sxs-lookup"><span data-stu-id="06326-134">String</span></span>|<span data-ttu-id="06326-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06326-135">Not yet documented</span></span>|
|<span data-ttu-id="06326-136">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="06326-136">notificationBody</span></span>|<span data-ttu-id="06326-137">String</span><span class="sxs-lookup"><span data-stu-id="06326-137">String</span></span>|<span data-ttu-id="06326-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06326-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06326-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="06326-139">Response</span></span>
<span data-ttu-id="06326-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06326-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06326-141">Пример</span><span class="sxs-lookup"><span data-stu-id="06326-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="06326-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="06326-142">Request</span></span>
<span data-ttu-id="06326-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06326-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="06326-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="06326-144">Response</span></span>
<span data-ttu-id="06326-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06326-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



