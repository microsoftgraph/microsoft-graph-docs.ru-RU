---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d23456c894fa1053a442247c7ca0f37adb246919
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536856"
---
# <a name="assign-action"></a><span data-ttu-id="6f946-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="6f946-103">assign action</span></span>

> <span data-ttu-id="6f946-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f946-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f946-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f946-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f946-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f946-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f946-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f946-107">Prerequisites</span></span>
<span data-ttu-id="6f946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f946-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f946-110">Permission type</span></span>|<span data-ttu-id="6f946-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f946-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f946-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f946-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f946-113">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="6f946-113">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="6f946-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f946-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="6f946-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6f946-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f946-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f946-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f946-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f946-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f946-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f946-118">Not supported.</span></span>|
|<span data-ttu-id="6f946-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f946-119">Application</span></span>||
| <span data-ttu-id="6f946-120">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="6f946-120">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="6f946-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f946-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="6f946-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6f946-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f946-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f946-123">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f946-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f946-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="6f946-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f946-125">Request headers</span></span>
|<span data-ttu-id="6f946-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f946-126">Header</span></span>|<span data-ttu-id="6f946-127">Значение</span><span class="sxs-lookup"><span data-stu-id="6f946-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f946-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f946-128">Authorization</span></span>|<span data-ttu-id="6f946-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f946-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f946-130">Accept</span><span class="sxs-lookup"><span data-stu-id="6f946-130">Accept</span></span>|<span data-ttu-id="6f946-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6f946-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f946-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f946-132">Request body</span></span>
<span data-ttu-id="6f946-133">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f946-133">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f946-134">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6f946-134">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f946-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f946-135">Property</span></span>|<span data-ttu-id="6f946-136">Тип</span><span class="sxs-lookup"><span data-stu-id="6f946-136">Type</span></span>|<span data-ttu-id="6f946-137">Описание</span><span class="sxs-lookup"><span data-stu-id="6f946-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f946-138">девицеидс</span><span class="sxs-lookup"><span data-stu-id="6f946-138">deviceIds</span></span>|<span data-ttu-id="6f946-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6f946-139">String collection</span></span>|<span data-ttu-id="6f946-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6f946-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f946-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f946-141">Response</span></span>
<span data-ttu-id="6f946-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f946-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6f946-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6f946-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f946-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f946-144">Request</span></span>
<span data-ttu-id="6f946-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f946-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f946-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f946-146">Response</span></span>
<span data-ttu-id="6f946-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f946-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






