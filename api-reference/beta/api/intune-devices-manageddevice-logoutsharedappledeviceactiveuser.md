---
title: Действие logoutSharedAppleDeviceActiveUser
description: Выход от имени активного пользователя общего устройства Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 452908dfaf5257e43da224fea1a19e0d3bd47a3f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167412"
---
# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="df797-103">Действие logoutSharedAppleDeviceActiveUser</span><span class="sxs-lookup"><span data-stu-id="df797-103">logoutSharedAppleDeviceActiveUser action</span></span>

> <span data-ttu-id="df797-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df797-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df797-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df797-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df797-106">Выход от имени активного пользователя общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="df797-106">Logout shared Apple device active user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df797-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="df797-107">Prerequisites</span></span>
<span data-ttu-id="df797-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="df797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df797-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df797-110">Permission type</span></span>|<span data-ttu-id="df797-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df797-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df797-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df797-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df797-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="df797-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="df797-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df797-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df797-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df797-115">Not supported.</span></span>|
|<span data-ttu-id="df797-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df797-116">Application</span></span>|<span data-ttu-id="df797-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df797-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df797-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df797-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="df797-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df797-119">Request headers</span></span>
|<span data-ttu-id="df797-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df797-120">Header</span></span>|<span data-ttu-id="df797-121">Значение</span><span class="sxs-lookup"><span data-stu-id="df797-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df797-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df797-122">Authorization</span></span>|<span data-ttu-id="df797-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="df797-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df797-124">Accept</span><span class="sxs-lookup"><span data-stu-id="df797-124">Accept</span></span>|<span data-ttu-id="df797-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df797-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df797-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df797-126">Request body</span></span>
<span data-ttu-id="df797-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df797-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df797-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="df797-128">Response</span></span>
<span data-ttu-id="df797-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df797-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df797-130">Пример</span><span class="sxs-lookup"><span data-stu-id="df797-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df797-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="df797-131">Request</span></span>
<span data-ttu-id="df797-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df797-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="df797-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="df797-133">Response</span></span>
<span data-ttu-id="df797-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df797-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




