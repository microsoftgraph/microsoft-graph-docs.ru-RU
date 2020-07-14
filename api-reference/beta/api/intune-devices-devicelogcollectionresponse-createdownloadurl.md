---
title: Действие createDownloadUrl
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a99fd6c09f213cde6494bcf912c5b6ffe58017
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124325"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="2e679-103">Действие createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="2e679-103">createDownloadUrl action</span></span>

<span data-ttu-id="2e679-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e679-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e679-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e679-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e679-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e679-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e679-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2e679-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e679-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e679-108">Prerequisites</span></span>
<span data-ttu-id="2e679-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2e679-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2e679-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e679-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e679-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e679-111">Permission type</span></span>|<span data-ttu-id="2e679-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e679-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e679-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e679-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e679-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e679-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2e679-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e679-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e679-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e679-116">Not supported.</span></span>|
|<span data-ttu-id="2e679-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e679-117">Application</span></span>|<span data-ttu-id="2e679-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e679-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e679-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e679-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="2e679-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e679-120">Request headers</span></span>
|<span data-ttu-id="2e679-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e679-121">Header</span></span>|<span data-ttu-id="2e679-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e679-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e679-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e679-123">Authorization</span></span>|<span data-ttu-id="2e679-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e679-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e679-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e679-125">Accept</span></span>|<span data-ttu-id="2e679-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e679-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e679-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e679-127">Request body</span></span>
<span data-ttu-id="2e679-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e679-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e679-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e679-129">Response</span></span>
<span data-ttu-id="2e679-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e679-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e679-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e679-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e679-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e679-132">Request</span></span>
<span data-ttu-id="2e679-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e679-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="2e679-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e679-134">Response</span></span>
<span data-ttu-id="2e679-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2e679-135">Here is an example of the response.</span></span> <span data-ttu-id="2e679-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2e679-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2e679-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2e679-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "https://example.com/createDownloadUrl/"
}
```



