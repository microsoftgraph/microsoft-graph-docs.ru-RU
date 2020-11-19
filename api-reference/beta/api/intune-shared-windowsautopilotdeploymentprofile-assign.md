---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b46184e7e201dbd31f4ced37b7547259fa0f54bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223656"
---
# <a name="assign-action"></a><span data-ttu-id="779f0-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="779f0-103">assign action</span></span>

<span data-ttu-id="779f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="779f0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="779f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="779f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="779f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="779f0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="779f0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="779f0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="779f0-108">Prerequisites</span></span>
<span data-ttu-id="779f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="779f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="779f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="779f0-111">Permission type</span></span>|<span data-ttu-id="779f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="779f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="779f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="779f0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="779f0-114">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="779f0-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="779f0-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779f0-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="779f0-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="779f0-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="779f0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779f0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="779f0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="779f0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="779f0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="779f0-119">Not supported.</span></span>|
|<span data-ttu-id="779f0-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="779f0-120">Application</span></span>||
| <span data-ttu-id="779f0-121">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="779f0-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="779f0-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779f0-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="779f0-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="779f0-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="779f0-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779f0-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="779f0-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="779f0-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="779f0-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="779f0-126">Request headers</span></span>
|<span data-ttu-id="779f0-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="779f0-127">Header</span></span>|<span data-ttu-id="779f0-128">Значение</span><span class="sxs-lookup"><span data-stu-id="779f0-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="779f0-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="779f0-129">Authorization</span></span>|<span data-ttu-id="779f0-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="779f0-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="779f0-131">Accept</span><span class="sxs-lookup"><span data-stu-id="779f0-131">Accept</span></span>|<span data-ttu-id="779f0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="779f0-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="779f0-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="779f0-133">Request body</span></span>
<span data-ttu-id="779f0-134">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="779f0-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="779f0-135">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="779f0-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="779f0-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="779f0-136">Property</span></span>|<span data-ttu-id="779f0-137">Тип</span><span class="sxs-lookup"><span data-stu-id="779f0-137">Type</span></span>|<span data-ttu-id="779f0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="779f0-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="779f0-139">девицеидс</span><span class="sxs-lookup"><span data-stu-id="779f0-139">deviceIds</span></span>|<span data-ttu-id="779f0-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="779f0-140">String collection</span></span>|<span data-ttu-id="779f0-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="779f0-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="779f0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="779f0-142">Response</span></span>
<span data-ttu-id="779f0-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="779f0-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="779f0-144">Пример</span><span class="sxs-lookup"><span data-stu-id="779f0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="779f0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="779f0-145">Request</span></span>
<span data-ttu-id="779f0-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="779f0-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="779f0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="779f0-147">Response</span></span>
<span data-ttu-id="779f0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="779f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







