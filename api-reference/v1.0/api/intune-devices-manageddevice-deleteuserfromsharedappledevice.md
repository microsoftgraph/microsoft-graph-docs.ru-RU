---
title: Действие deleteUserFromSharedAppleDevice
description: Удаление пользователя на общем устройстве Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2b6fbbac6718f47bea0dafbfda1b2a76715dc95
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753696"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="ee57b-103">Действие deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="ee57b-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="ee57b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee57b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee57b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee57b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee57b-106">Удаление пользователя на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="ee57b-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee57b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee57b-107">Prerequisites</span></span>
<span data-ttu-id="ee57b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee57b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee57b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee57b-110">Permission type</span></span>|<span data-ttu-id="ee57b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee57b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee57b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee57b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee57b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ee57b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ee57b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee57b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee57b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee57b-115">Not supported.</span></span>|
|<span data-ttu-id="ee57b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ee57b-116">Application</span></span>|<span data-ttu-id="ee57b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ee57b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee57b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee57b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="ee57b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee57b-119">Request headers</span></span>
|<span data-ttu-id="ee57b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee57b-120">Header</span></span>|<span data-ttu-id="ee57b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee57b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee57b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee57b-122">Authorization</span></span>|<span data-ttu-id="ee57b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee57b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee57b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee57b-124">Accept</span></span>|<span data-ttu-id="ee57b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee57b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee57b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee57b-126">Request body</span></span>
<span data-ttu-id="ee57b-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee57b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee57b-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ee57b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee57b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee57b-129">Property</span></span>|<span data-ttu-id="ee57b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee57b-130">Type</span></span>|<span data-ttu-id="ee57b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee57b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee57b-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee57b-132">userPrincipalName</span></span>|<span data-ttu-id="ee57b-133">String</span><span class="sxs-lookup"><span data-stu-id="ee57b-133">String</span></span>|<span data-ttu-id="ee57b-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ee57b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ee57b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee57b-135">Response</span></span>
<span data-ttu-id="ee57b-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee57b-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee57b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ee57b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee57b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee57b-138">Request</span></span>
<span data-ttu-id="ee57b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee57b-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ee57b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee57b-140">Response</span></span>
<span data-ttu-id="ee57b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee57b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




