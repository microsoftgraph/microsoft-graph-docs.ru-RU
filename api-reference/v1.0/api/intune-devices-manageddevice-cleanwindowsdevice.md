---
title: Действие cleanWindowsDevice
description: Очистка устройства с Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b21b986c3ffeb1338461e7fdffd7829a7eae1348
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364517"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="03f7c-103">Действие cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="03f7c-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="03f7c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03f7c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03f7c-105">Очистка устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="03f7c-105">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03f7c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="03f7c-106">Prerequisites</span></span>
<span data-ttu-id="03f7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03f7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03f7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03f7c-109">Permission type</span></span>|<span data-ttu-id="03f7c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03f7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03f7c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03f7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03f7c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="03f7c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="03f7c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03f7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03f7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f7c-114">Not supported.</span></span>|
|<span data-ttu-id="03f7c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03f7c-115">Application</span></span>|<span data-ttu-id="03f7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03f7c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03f7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="03f7c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03f7c-118">Request headers</span></span>
|<span data-ttu-id="03f7c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03f7c-119">Header</span></span>|<span data-ttu-id="03f7c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="03f7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03f7c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03f7c-121">Authorization</span></span>|<span data-ttu-id="03f7c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03f7c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="03f7c-123">Accept</span></span>|<span data-ttu-id="03f7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="03f7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03f7c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03f7c-125">Request body</span></span>
<span data-ttu-id="03f7c-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03f7c-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="03f7c-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="03f7c-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="03f7c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="03f7c-128">Property</span></span>|<span data-ttu-id="03f7c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="03f7c-129">Type</span></span>|<span data-ttu-id="03f7c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="03f7c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f7c-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="03f7c-131">keepUserData</span></span>|<span data-ttu-id="03f7c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="03f7c-132">Boolean</span></span>|<span data-ttu-id="03f7c-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="03f7c-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="03f7c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="03f7c-134">Response</span></span>
<span data-ttu-id="03f7c-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03f7c-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="03f7c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="03f7c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="03f7c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="03f7c-137">Request</span></span>
<span data-ttu-id="03f7c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03f7c-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="03f7c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="03f7c-139">Response</span></span>
<span data-ttu-id="03f7c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03f7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




