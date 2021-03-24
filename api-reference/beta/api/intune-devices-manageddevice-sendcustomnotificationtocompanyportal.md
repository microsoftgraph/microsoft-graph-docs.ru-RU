---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0809f32ff83982f4964e68026f54872c6592be6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136274"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="2bd27-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2bd27-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="2bd27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bd27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bd27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bd27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bd27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bd27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bd27-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2bd27-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bd27-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2bd27-108">Prerequisites</span></span>
<span data-ttu-id="2bd27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bd27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bd27-111">Permission type</span></span>|<span data-ttu-id="2bd27-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bd27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bd27-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bd27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bd27-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bd27-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2bd27-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bd27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bd27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bd27-116">Not supported.</span></span>|
|<span data-ttu-id="2bd27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2bd27-117">Application</span></span>|<span data-ttu-id="2bd27-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bd27-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bd27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bd27-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2bd27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2bd27-120">Request headers</span></span>
|<span data-ttu-id="2bd27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bd27-121">Header</span></span>|<span data-ttu-id="2bd27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2bd27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bd27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bd27-123">Authorization</span></span>|<span data-ttu-id="2bd27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bd27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bd27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2bd27-125">Accept</span></span>|<span data-ttu-id="2bd27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bd27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bd27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bd27-127">Request body</span></span>
<span data-ttu-id="2bd27-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bd27-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2bd27-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2bd27-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2bd27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bd27-130">Property</span></span>|<span data-ttu-id="2bd27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2bd27-131">Type</span></span>|<span data-ttu-id="2bd27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2bd27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bd27-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="2bd27-133">notificationTitle</span></span>|<span data-ttu-id="2bd27-134">String</span><span class="sxs-lookup"><span data-stu-id="2bd27-134">String</span></span>|<span data-ttu-id="2bd27-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2bd27-135">Not yet documented</span></span>|
|<span data-ttu-id="2bd27-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="2bd27-136">notificationBody</span></span>|<span data-ttu-id="2bd27-137">String</span><span class="sxs-lookup"><span data-stu-id="2bd27-137">String</span></span>|<span data-ttu-id="2bd27-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2bd27-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2bd27-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bd27-139">Response</span></span>
<span data-ttu-id="2bd27-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2bd27-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2bd27-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2bd27-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bd27-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bd27-142">Request</span></span>
<span data-ttu-id="2bd27-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bd27-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="2bd27-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bd27-144">Response</span></span>
<span data-ttu-id="2bd27-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bd27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




