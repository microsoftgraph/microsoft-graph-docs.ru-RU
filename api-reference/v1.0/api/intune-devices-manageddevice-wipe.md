---
title: Действие wipe
description: Очистка устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20ebe11dce6847066148f06a77bffa970e3a1b1e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919822"
---
# <a name="wipe-action"></a><span data-ttu-id="3912f-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="3912f-103">wipe action</span></span>

> <span data-ttu-id="3912f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3912f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3912f-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="3912f-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3912f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3912f-106">Prerequisites</span></span>
<span data-ttu-id="3912f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3912f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3912f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3912f-109">Permission type</span></span>|<span data-ttu-id="3912f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3912f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3912f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3912f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3912f-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3912f-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3912f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3912f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3912f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3912f-114">Not supported.</span></span>|
|<span data-ttu-id="3912f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3912f-115">Application</span></span>|<span data-ttu-id="3912f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3912f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3912f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3912f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="3912f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3912f-118">Request headers</span></span>
|<span data-ttu-id="3912f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3912f-119">Header</span></span>|<span data-ttu-id="3912f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3912f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3912f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3912f-121">Authorization</span></span>|<span data-ttu-id="3912f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3912f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3912f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3912f-123">Accept</span></span>|<span data-ttu-id="3912f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3912f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3912f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3912f-125">Request body</span></span>
<span data-ttu-id="3912f-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3912f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3912f-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3912f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3912f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3912f-128">Property</span></span>|<span data-ttu-id="3912f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3912f-129">Type</span></span>|<span data-ttu-id="3912f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3912f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3912f-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="3912f-131">keepEnrollmentData</span></span>|<span data-ttu-id="3912f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="3912f-132">Boolean</span></span>|<span data-ttu-id="3912f-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3912f-133">Not yet documented</span></span>|
|<span data-ttu-id="3912f-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="3912f-134">keepUserData</span></span>|<span data-ttu-id="3912f-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3912f-135">Boolean</span></span>|<span data-ttu-id="3912f-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3912f-136">Not yet documented</span></span>|
|<span data-ttu-id="3912f-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="3912f-137">macOsUnlockCode</span></span>|<span data-ttu-id="3912f-138">String</span><span class="sxs-lookup"><span data-stu-id="3912f-138">String</span></span>|<span data-ttu-id="3912f-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3912f-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3912f-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="3912f-140">Response</span></span>
<span data-ttu-id="3912f-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3912f-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3912f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3912f-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="3912f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3912f-143">Request</span></span>
<span data-ttu-id="3912f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3912f-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="3912f-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="3912f-145">Response</span></span>
<span data-ttu-id="3912f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3912f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



