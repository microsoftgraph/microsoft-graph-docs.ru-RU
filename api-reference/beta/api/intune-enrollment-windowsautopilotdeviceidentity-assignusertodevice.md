---
title: Действие assignUserToDevice
description: Назначение пользователям автопилотных устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3a1dcfee91b93b9c0fcf3bdf1e5bdf25b387c24
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967827"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="46caa-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="46caa-103">assignUserToDevice action</span></span>

> <span data-ttu-id="46caa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46caa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46caa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46caa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46caa-106">Назначение пользователям автопилотных устройств.</span><span class="sxs-lookup"><span data-stu-id="46caa-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46caa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46caa-107">Prerequisites</span></span>
<span data-ttu-id="46caa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46caa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46caa-110">Permission type</span></span>|<span data-ttu-id="46caa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46caa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46caa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46caa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46caa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46caa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46caa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46caa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46caa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46caa-115">Not supported.</span></span>|
|<span data-ttu-id="46caa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46caa-116">Application</span></span>|<span data-ttu-id="46caa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46caa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46caa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46caa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="46caa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46caa-119">Request headers</span></span>
|<span data-ttu-id="46caa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46caa-120">Header</span></span>|<span data-ttu-id="46caa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46caa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46caa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46caa-122">Authorization</span></span>|<span data-ttu-id="46caa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46caa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46caa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46caa-124">Accept</span></span>|<span data-ttu-id="46caa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46caa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46caa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46caa-126">Request body</span></span>
<span data-ttu-id="46caa-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46caa-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="46caa-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="46caa-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="46caa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46caa-129">Property</span></span>|<span data-ttu-id="46caa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46caa-130">Type</span></span>|<span data-ttu-id="46caa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46caa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46caa-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46caa-132">userPrincipalName</span></span>|<span data-ttu-id="46caa-133">String</span><span class="sxs-lookup"><span data-stu-id="46caa-133">String</span></span>|<span data-ttu-id="46caa-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="46caa-134">Not yet documented</span></span>|
|<span data-ttu-id="46caa-135">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="46caa-135">addressableUserName</span></span>|<span data-ttu-id="46caa-136">String</span><span class="sxs-lookup"><span data-stu-id="46caa-136">String</span></span>|<span data-ttu-id="46caa-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="46caa-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="46caa-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="46caa-138">Response</span></span>
<span data-ttu-id="46caa-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46caa-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46caa-140">Пример</span><span class="sxs-lookup"><span data-stu-id="46caa-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="46caa-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="46caa-141">Request</span></span>
<span data-ttu-id="46caa-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46caa-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="46caa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="46caa-143">Response</span></span>
<span data-ttu-id="46caa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46caa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




