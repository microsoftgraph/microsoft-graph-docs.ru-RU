---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2c13bd6798c6a73b953b3f273c76a9dee1365ab
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868073"
---
# <a name="assign-action"></a><span data-ttu-id="30340-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="30340-103">assign action</span></span>

<span data-ttu-id="30340-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30340-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30340-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30340-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30340-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30340-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30340-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="30340-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30340-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30340-108">Prerequisites</span></span>
<span data-ttu-id="30340-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30340-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30340-111">Permission type</span></span>|<span data-ttu-id="30340-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30340-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30340-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30340-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="30340-114">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="30340-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="30340-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30340-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="30340-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="30340-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="30340-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30340-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30340-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30340-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30340-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30340-119">Not supported.</span></span>|
|<span data-ttu-id="30340-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="30340-120">Application</span></span>||
| <span data-ttu-id="30340-121">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="30340-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="30340-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30340-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="30340-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="30340-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="30340-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30340-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30340-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30340-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="30340-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30340-126">Request headers</span></span>
|<span data-ttu-id="30340-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30340-127">Header</span></span>|<span data-ttu-id="30340-128">Значение</span><span class="sxs-lookup"><span data-stu-id="30340-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30340-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30340-129">Authorization</span></span>|<span data-ttu-id="30340-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30340-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30340-131">Accept</span><span class="sxs-lookup"><span data-stu-id="30340-131">Accept</span></span>|<span data-ttu-id="30340-132">application/json</span><span class="sxs-lookup"><span data-stu-id="30340-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30340-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30340-133">Request body</span></span>
<span data-ttu-id="30340-134">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30340-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="30340-135">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="30340-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="30340-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="30340-136">Property</span></span>|<span data-ttu-id="30340-137">Тип</span><span class="sxs-lookup"><span data-stu-id="30340-137">Type</span></span>|<span data-ttu-id="30340-138">Описание</span><span class="sxs-lookup"><span data-stu-id="30340-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30340-139">deviceIds</span><span class="sxs-lookup"><span data-stu-id="30340-139">deviceIds</span></span>|<span data-ttu-id="30340-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="30340-140">String collection</span></span>|<span data-ttu-id="30340-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="30340-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="30340-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="30340-142">Response</span></span>
<span data-ttu-id="30340-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="30340-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="30340-144">Пример</span><span class="sxs-lookup"><span data-stu-id="30340-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="30340-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="30340-145">Request</span></span>
<span data-ttu-id="30340-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30340-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30340-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="30340-147">Response</span></span>
<span data-ttu-id="30340-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30340-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







