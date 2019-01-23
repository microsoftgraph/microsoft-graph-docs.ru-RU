---
title: Действие wipe
description: Очистка устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56ee058ee4ea6c5760707f895d626b35163c68ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398711"
---
# <a name="wipe-action"></a><span data-ttu-id="90bb4-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="90bb4-103">wipe action</span></span>

> <span data-ttu-id="90bb4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90bb4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90bb4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90bb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90bb4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90bb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90bb4-107">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="90bb4-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90bb4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="90bb4-108">Prerequisites</span></span>
<span data-ttu-id="90bb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="90bb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90bb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90bb4-111">Permission type</span></span>|<span data-ttu-id="90bb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90bb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90bb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90bb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90bb4-114">DeviceManagementManagedDevices.PriviligedOperation.All DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90bb4-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90bb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90bb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90bb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90bb4-116">Not supported.</span></span>|
|<span data-ttu-id="90bb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90bb4-117">Application</span></span>|<span data-ttu-id="90bb4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90bb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90bb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90bb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="90bb4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90bb4-120">Request headers</span></span>
|<span data-ttu-id="90bb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90bb4-121">Header</span></span>|<span data-ttu-id="90bb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90bb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90bb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90bb4-123">Authorization</span></span>|<span data-ttu-id="90bb4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="90bb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90bb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90bb4-125">Accept</span></span>|<span data-ttu-id="90bb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90bb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90bb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90bb4-127">Request body</span></span>
<span data-ttu-id="90bb4-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90bb4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="90bb4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="90bb4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="90bb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="90bb4-130">Property</span></span>|<span data-ttu-id="90bb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="90bb4-131">Type</span></span>|<span data-ttu-id="90bb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90bb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90bb4-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="90bb4-133">keepEnrollmentData</span></span>|<span data-ttu-id="90bb4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="90bb4-134">Boolean</span></span>|<span data-ttu-id="90bb4-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90bb4-135">Not yet documented</span></span>|
|<span data-ttu-id="90bb4-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="90bb4-136">keepUserData</span></span>|<span data-ttu-id="90bb4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="90bb4-137">Boolean</span></span>|<span data-ttu-id="90bb4-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90bb4-138">Not yet documented</span></span>|
|<span data-ttu-id="90bb4-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="90bb4-139">macOsUnlockCode</span></span>|<span data-ttu-id="90bb4-140">String</span><span class="sxs-lookup"><span data-stu-id="90bb4-140">String</span></span>|<span data-ttu-id="90bb4-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90bb4-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="90bb4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="90bb4-142">Response</span></span>
<span data-ttu-id="90bb4-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90bb4-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90bb4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="90bb4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="90bb4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="90bb4-145">Request</span></span>
<span data-ttu-id="90bb4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90bb4-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="90bb4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="90bb4-147">Response</span></span>
<span data-ttu-id="90bb4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="90bb4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




