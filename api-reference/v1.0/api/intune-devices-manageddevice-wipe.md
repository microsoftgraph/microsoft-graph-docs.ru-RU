---
title: Действие wipe
description: Очистка устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3249421de530cdc8e5e7f9c5a90676572c5b7ae9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983234"
---
# <a name="wipe-action"></a><span data-ttu-id="234cf-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="234cf-103">wipe action</span></span>

> <span data-ttu-id="234cf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="234cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="234cf-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="234cf-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="234cf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="234cf-106">Prerequisites</span></span>
<span data-ttu-id="234cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="234cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="234cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="234cf-109">Permission type</span></span>|<span data-ttu-id="234cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="234cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="234cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="234cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="234cf-112">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="234cf-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="234cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="234cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="234cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234cf-114">Not supported.</span></span>|
|<span data-ttu-id="234cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="234cf-115">Application</span></span>|<span data-ttu-id="234cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="234cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="234cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="234cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="234cf-118">Request headers</span></span>
|<span data-ttu-id="234cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="234cf-119">Header</span></span>|<span data-ttu-id="234cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="234cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="234cf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="234cf-121">Authorization</span></span>|<span data-ttu-id="234cf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="234cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="234cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="234cf-123">Accept</span></span>|<span data-ttu-id="234cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="234cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="234cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="234cf-125">Request body</span></span>
<span data-ttu-id="234cf-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="234cf-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="234cf-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="234cf-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="234cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="234cf-128">Property</span></span>|<span data-ttu-id="234cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="234cf-129">Type</span></span>|<span data-ttu-id="234cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="234cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="234cf-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="234cf-131">keepEnrollmentData</span></span>|<span data-ttu-id="234cf-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="234cf-132">Boolean</span></span>|<span data-ttu-id="234cf-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="234cf-133">Not yet documented</span></span>|
|<span data-ttu-id="234cf-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="234cf-134">keepUserData</span></span>|<span data-ttu-id="234cf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="234cf-135">Boolean</span></span>|<span data-ttu-id="234cf-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="234cf-136">Not yet documented</span></span>|
|<span data-ttu-id="234cf-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="234cf-137">macOsUnlockCode</span></span>|<span data-ttu-id="234cf-138">String</span><span class="sxs-lookup"><span data-stu-id="234cf-138">String</span></span>|<span data-ttu-id="234cf-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="234cf-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="234cf-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="234cf-140">Response</span></span>
<span data-ttu-id="234cf-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="234cf-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="234cf-142">Пример</span><span class="sxs-lookup"><span data-stu-id="234cf-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="234cf-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="234cf-143">Request</span></span>
<span data-ttu-id="234cf-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="234cf-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="234cf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="234cf-145">Response</span></span>
<span data-ttu-id="234cf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="234cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



