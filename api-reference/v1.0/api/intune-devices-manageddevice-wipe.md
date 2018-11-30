---
title: Действие wipe
description: Очистка устройства
ms.openlocfilehash: 377b1c299885d042dd372f661410ea43d20fd021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026163"
---
# <a name="wipe-action"></a><span data-ttu-id="11eb6-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="11eb6-103">wipe action</span></span>

> <span data-ttu-id="11eb6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11eb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11eb6-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="11eb6-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11eb6-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="11eb6-106">Prerequisites</span></span>
<span data-ttu-id="11eb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11eb6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11eb6-109">Permission type</span></span>|<span data-ttu-id="11eb6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11eb6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11eb6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11eb6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11eb6-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="11eb6-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="11eb6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11eb6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11eb6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11eb6-114">Not supported.</span></span>|
|<span data-ttu-id="11eb6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11eb6-115">Application</span></span>|<span data-ttu-id="11eb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11eb6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11eb6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11eb6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="11eb6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11eb6-118">Request headers</span></span>
|<span data-ttu-id="11eb6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11eb6-119">Header</span></span>|<span data-ttu-id="11eb6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11eb6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11eb6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11eb6-121">Authorization</span></span>|<span data-ttu-id="11eb6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="11eb6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11eb6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11eb6-123">Accept</span></span>|<span data-ttu-id="11eb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11eb6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11eb6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11eb6-125">Request body</span></span>
<span data-ttu-id="11eb6-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11eb6-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="11eb6-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="11eb6-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="11eb6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="11eb6-128">Property</span></span>|<span data-ttu-id="11eb6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11eb6-129">Type</span></span>|<span data-ttu-id="11eb6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11eb6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11eb6-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="11eb6-131">keepEnrollmentData</span></span>|<span data-ttu-id="11eb6-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="11eb6-132">Boolean</span></span>|<span data-ttu-id="11eb6-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11eb6-133">Not yet documented</span></span>|
|<span data-ttu-id="11eb6-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="11eb6-134">keepUserData</span></span>|<span data-ttu-id="11eb6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="11eb6-135">Boolean</span></span>|<span data-ttu-id="11eb6-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11eb6-136">Not yet documented</span></span>|
|<span data-ttu-id="11eb6-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="11eb6-137">macOsUnlockCode</span></span>|<span data-ttu-id="11eb6-138">String</span><span class="sxs-lookup"><span data-stu-id="11eb6-138">String</span></span>|<span data-ttu-id="11eb6-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11eb6-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="11eb6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="11eb6-140">Response</span></span>
<span data-ttu-id="11eb6-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="11eb6-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11eb6-142">Пример</span><span class="sxs-lookup"><span data-stu-id="11eb6-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="11eb6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="11eb6-143">Request</span></span>
<span data-ttu-id="11eb6-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11eb6-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11eb6-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="11eb6-145">Response</span></span>
<span data-ttu-id="11eb6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="11eb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



