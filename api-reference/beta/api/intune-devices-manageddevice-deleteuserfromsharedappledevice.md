---
title: Действие deleteUserFromSharedAppleDevice
description: Удаление пользователя на общем устройстве Apple
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f764325d68b2c82cd36ed806c78424d21d728fa7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403723"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="a63ac-103">Действие deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="a63ac-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="a63ac-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a63ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a63ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a63ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a63ac-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a63ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a63ac-107">Удаление пользователя на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="a63ac-107">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a63ac-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a63ac-108">Prerequisites</span></span>
<span data-ttu-id="a63ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a63ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a63ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a63ac-111">Permission type</span></span>|<span data-ttu-id="a63ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a63ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a63ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a63ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a63ac-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a63ac-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a63ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a63ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a63ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a63ac-116">Not supported.</span></span>|
|<span data-ttu-id="a63ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a63ac-117">Application</span></span>|<span data-ttu-id="a63ac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a63ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a63ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a63ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="a63ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a63ac-120">Request headers</span></span>
|<span data-ttu-id="a63ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a63ac-121">Header</span></span>|<span data-ttu-id="a63ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a63ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a63ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a63ac-123">Authorization</span></span>|<span data-ttu-id="a63ac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a63ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a63ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a63ac-125">Accept</span></span>|<span data-ttu-id="a63ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a63ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a63ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a63ac-127">Request body</span></span>
<span data-ttu-id="a63ac-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a63ac-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a63ac-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a63ac-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a63ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a63ac-130">Property</span></span>|<span data-ttu-id="a63ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a63ac-131">Type</span></span>|<span data-ttu-id="a63ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a63ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a63ac-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a63ac-133">userPrincipalName</span></span>|<span data-ttu-id="a63ac-134">String</span><span class="sxs-lookup"><span data-stu-id="a63ac-134">String</span></span>|<span data-ttu-id="a63ac-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a63ac-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a63ac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a63ac-136">Response</span></span>
<span data-ttu-id="a63ac-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a63ac-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a63ac-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a63ac-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a63ac-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a63ac-139">Request</span></span>
<span data-ttu-id="a63ac-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a63ac-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a63ac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a63ac-141">Response</span></span>
<span data-ttu-id="a63ac-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a63ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




