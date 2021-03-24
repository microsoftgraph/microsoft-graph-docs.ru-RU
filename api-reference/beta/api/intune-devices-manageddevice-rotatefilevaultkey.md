---
title: действия rotateFileVaultKey
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64264d80d03fb306104a94cd019934ce4a652e37
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136295"
---
# <a name="rotatefilevaultkey-action"></a><span data-ttu-id="717de-103">действия rotateFileVaultKey</span><span class="sxs-lookup"><span data-stu-id="717de-103">rotateFileVaultKey action</span></span>

<span data-ttu-id="717de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="717de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="717de-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="717de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="717de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="717de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="717de-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="717de-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="717de-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="717de-108">Prerequisites</span></span>
<span data-ttu-id="717de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="717de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="717de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="717de-111">Permission type</span></span>|<span data-ttu-id="717de-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="717de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="717de-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="717de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="717de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="717de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="717de-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="717de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="717de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="717de-116">Not supported.</span></span>|
|<span data-ttu-id="717de-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="717de-117">Application</span></span>|<span data-ttu-id="717de-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="717de-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="717de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="717de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

## <a name="request-headers"></a><span data-ttu-id="717de-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="717de-120">Request headers</span></span>
|<span data-ttu-id="717de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="717de-121">Header</span></span>|<span data-ttu-id="717de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="717de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="717de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="717de-123">Authorization</span></span>|<span data-ttu-id="717de-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="717de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="717de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="717de-125">Accept</span></span>|<span data-ttu-id="717de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="717de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="717de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="717de-127">Request body</span></span>
<span data-ttu-id="717de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="717de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="717de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="717de-129">Response</span></span>
<span data-ttu-id="717de-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="717de-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="717de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="717de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="717de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="717de-132">Request</span></span>
<span data-ttu-id="717de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="717de-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

### <a name="response"></a><span data-ttu-id="717de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="717de-134">Response</span></span>
<span data-ttu-id="717de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="717de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




