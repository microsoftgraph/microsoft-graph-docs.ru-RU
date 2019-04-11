---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f852d446ef0a931233aa2cb8bb4c9a1fc97295bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803880"
---
# <a name="assign-action"></a><span data-ttu-id="1a585-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="1a585-103">assign action</span></span>

> <span data-ttu-id="1a585-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a585-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a585-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a585-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a585-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1a585-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a585-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a585-107">Prerequisites</span></span>
<span data-ttu-id="1a585-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a585-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a585-110">Permission type</span></span>|<span data-ttu-id="1a585-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a585-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a585-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a585-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a585-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a585-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a585-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a585-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a585-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a585-115">Not supported.</span></span>|
|<span data-ttu-id="1a585-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a585-116">Application</span></span>|<span data-ttu-id="1a585-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a585-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a585-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a585-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="1a585-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a585-119">Request headers</span></span>
|<span data-ttu-id="1a585-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a585-120">Header</span></span>|<span data-ttu-id="1a585-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a585-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a585-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a585-122">Authorization</span></span>|<span data-ttu-id="1a585-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a585-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a585-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a585-124">Accept</span></span>|<span data-ttu-id="1a585-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a585-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a585-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a585-126">Request body</span></span>
<span data-ttu-id="1a585-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a585-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1a585-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="1a585-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1a585-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a585-129">Property</span></span>|<span data-ttu-id="1a585-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a585-130">Type</span></span>|<span data-ttu-id="1a585-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a585-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a585-132">Девицеидс</span><span class="sxs-lookup"><span data-stu-id="1a585-132">deviceIds</span></span>|<span data-ttu-id="1a585-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1a585-133">String collection</span></span>|<span data-ttu-id="1a585-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1a585-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1a585-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a585-135">Response</span></span>
<span data-ttu-id="1a585-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1a585-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1a585-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1a585-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a585-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a585-138">Request</span></span>
<span data-ttu-id="1a585-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a585-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a585-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a585-140">Response</span></span>
<span data-ttu-id="1a585-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a585-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





