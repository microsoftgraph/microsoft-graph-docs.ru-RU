---
title: Действие windowsDefenderScan
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d0839b8f92a2df97436ac589669f2870a87608f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018584"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="a07e2-103">Действие windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="a07e2-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="a07e2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a07e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a07e2-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a07e2-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a07e2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a07e2-106">Prerequisites</span></span>
<span data-ttu-id="a07e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a07e2-109">Permission type</span></span>|<span data-ttu-id="a07e2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a07e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a07e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a07e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a07e2-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a07e2-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a07e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a07e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a07e2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a07e2-114">Not supported.</span></span>|
|<span data-ttu-id="a07e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a07e2-115">Application</span></span>|<span data-ttu-id="a07e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a07e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a07e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a07e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="a07e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a07e2-118">Request headers</span></span>
|<span data-ttu-id="a07e2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a07e2-119">Header</span></span>|<span data-ttu-id="a07e2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a07e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a07e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a07e2-121">Authorization</span></span>|<span data-ttu-id="a07e2-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a07e2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a07e2-123">Accept</span></span>|<span data-ttu-id="a07e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a07e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a07e2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a07e2-125">Request body</span></span>
<span data-ttu-id="a07e2-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a07e2-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a07e2-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a07e2-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a07e2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a07e2-128">Property</span></span>|<span data-ttu-id="a07e2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a07e2-129">Type</span></span>|<span data-ttu-id="a07e2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a07e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a07e2-131">quickScan</span><span class="sxs-lookup"><span data-stu-id="a07e2-131">quickScan</span></span>|<span data-ttu-id="a07e2-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="a07e2-132">Boolean</span></span>|<span data-ttu-id="a07e2-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a07e2-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a07e2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a07e2-134">Response</span></span>
<span data-ttu-id="a07e2-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a07e2-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a07e2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a07e2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a07e2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a07e2-137">Request</span></span>
<span data-ttu-id="a07e2-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a07e2-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="a07e2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07e2-139">Response</span></span>
<span data-ttu-id="a07e2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a07e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



