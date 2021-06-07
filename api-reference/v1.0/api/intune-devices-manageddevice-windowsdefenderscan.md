---
title: Действие windowsDefenderScan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abd1cd6bfe2d4d0f9ebb96e433ad0db191b76366
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752632"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="992e4-103">Действие windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="992e4-103">windowsDefenderScan action</span></span>

<span data-ttu-id="992e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="992e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="992e4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="992e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="992e4-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="992e4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="992e4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="992e4-107">Prerequisites</span></span>
<span data-ttu-id="992e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="992e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="992e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="992e4-110">Permission type</span></span>|<span data-ttu-id="992e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="992e4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="992e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="992e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="992e4-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="992e4-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="992e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="992e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="992e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="992e4-115">Not supported.</span></span>|
|<span data-ttu-id="992e4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="992e4-116">Application</span></span>|<span data-ttu-id="992e4-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="992e4-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="992e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="992e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="992e4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="992e4-119">Request headers</span></span>
|<span data-ttu-id="992e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="992e4-120">Header</span></span>|<span data-ttu-id="992e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="992e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="992e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="992e4-122">Authorization</span></span>|<span data-ttu-id="992e4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="992e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="992e4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="992e4-124">Accept</span></span>|<span data-ttu-id="992e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="992e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="992e4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="992e4-126">Request body</span></span>
<span data-ttu-id="992e4-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="992e4-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="992e4-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="992e4-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="992e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="992e4-129">Property</span></span>|<span data-ttu-id="992e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="992e4-130">Type</span></span>|<span data-ttu-id="992e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="992e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="992e4-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="992e4-132">quickScan</span></span>|<span data-ttu-id="992e4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="992e4-133">Boolean</span></span>|<span data-ttu-id="992e4-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="992e4-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="992e4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="992e4-135">Response</span></span>
<span data-ttu-id="992e4-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="992e4-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="992e4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="992e4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="992e4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="992e4-138">Request</span></span>
<span data-ttu-id="992e4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="992e4-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="992e4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="992e4-140">Response</span></span>
<span data-ttu-id="992e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="992e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




