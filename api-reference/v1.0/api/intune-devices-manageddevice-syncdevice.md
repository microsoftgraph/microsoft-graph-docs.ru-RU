---
title: Действие syncDevice
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ebe51c8d162111bc6d42366873b8631fdc33e9d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364293"
---
# <a name="syncdevice-action"></a><span data-ttu-id="c8309-103">Действие syncDevice</span><span class="sxs-lookup"><span data-stu-id="c8309-103">syncDevice action</span></span>

> <span data-ttu-id="c8309-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8309-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8309-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c8309-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8309-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8309-106">Prerequisites</span></span>
<span data-ttu-id="c8309-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8309-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8309-109">Permission type</span></span>|<span data-ttu-id="c8309-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8309-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8309-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8309-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8309-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c8309-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c8309-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8309-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8309-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8309-114">Not supported.</span></span>|
|<span data-ttu-id="c8309-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8309-115">Application</span></span>|<span data-ttu-id="c8309-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8309-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8309-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8309-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="c8309-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8309-118">Request headers</span></span>
|<span data-ttu-id="c8309-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8309-119">Header</span></span>|<span data-ttu-id="c8309-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c8309-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8309-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8309-121">Authorization</span></span>|<span data-ttu-id="c8309-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8309-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8309-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c8309-123">Accept</span></span>|<span data-ttu-id="c8309-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8309-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8309-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8309-125">Request body</span></span>
<span data-ttu-id="c8309-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8309-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8309-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8309-127">Response</span></span>
<span data-ttu-id="c8309-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8309-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8309-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c8309-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8309-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8309-130">Request</span></span>
<span data-ttu-id="c8309-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8309-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="c8309-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8309-132">Response</span></span>
<span data-ttu-id="c8309-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8309-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




