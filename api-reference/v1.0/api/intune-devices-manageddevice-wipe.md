---
title: Действие wipe
description: Очистка устройства
author: tfitzmac
ms.openlocfilehash: 6ac3c21b517523d46cfc2958a661d058a86d708e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311419"
---
# <a name="wipe-action"></a><span data-ttu-id="a59e4-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="a59e4-103">wipe action</span></span>

> <span data-ttu-id="a59e4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a59e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a59e4-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="a59e4-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a59e4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a59e4-106">Prerequisites</span></span>
<span data-ttu-id="a59e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a59e4-109">Permission type</span></span>|<span data-ttu-id="a59e4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a59e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a59e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a59e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a59e4-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a59e4-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a59e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a59e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a59e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a59e4-114">Not supported.</span></span>|
|<span data-ttu-id="a59e4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a59e4-115">Application</span></span>|<span data-ttu-id="a59e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a59e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a59e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a59e4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="a59e4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a59e4-118">Request headers</span></span>
|<span data-ttu-id="a59e4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a59e4-119">Header</span></span>|<span data-ttu-id="a59e4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a59e4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a59e4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a59e4-121">Authorization</span></span>|<span data-ttu-id="a59e4-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a59e4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a59e4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a59e4-123">Accept</span></span>|<span data-ttu-id="a59e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a59e4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59e4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a59e4-125">Request body</span></span>
<span data-ttu-id="a59e4-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a59e4-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a59e4-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a59e4-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a59e4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a59e4-128">Property</span></span>|<span data-ttu-id="a59e4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a59e4-129">Type</span></span>|<span data-ttu-id="a59e4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a59e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59e4-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="a59e4-131">keepEnrollmentData</span></span>|<span data-ttu-id="a59e4-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59e4-132">Boolean</span></span>|<span data-ttu-id="a59e4-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a59e4-133">Not yet documented</span></span>|
|<span data-ttu-id="a59e4-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="a59e4-134">keepUserData</span></span>|<span data-ttu-id="a59e4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59e4-135">Boolean</span></span>|<span data-ttu-id="a59e4-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a59e4-136">Not yet documented</span></span>|
|<span data-ttu-id="a59e4-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="a59e4-137">macOsUnlockCode</span></span>|<span data-ttu-id="a59e4-138">String</span><span class="sxs-lookup"><span data-stu-id="a59e4-138">String</span></span>|<span data-ttu-id="a59e4-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a59e4-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a59e4-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="a59e4-140">Response</span></span>
<span data-ttu-id="a59e4-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a59e4-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a59e4-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a59e4-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="a59e4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a59e4-143">Request</span></span>
<span data-ttu-id="a59e4-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a59e4-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a59e4-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="a59e4-145">Response</span></span>
<span data-ttu-id="a59e4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a59e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



