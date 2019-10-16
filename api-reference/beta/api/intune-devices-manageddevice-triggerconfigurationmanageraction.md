---
title: действие Тригжерконфигуратионманажерактион
description: Действие триггера в клиенте Конфигуратионманажер
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0533b65a2807c608ac0f5daa9ccabb44011a2f14
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528250"
---
# <a name="triggerconfigurationmanageraction-action"></a><span data-ttu-id="33808-103">действие Тригжерконфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="33808-103">triggerConfigurationManagerAction action</span></span>

> <span data-ttu-id="33808-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33808-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33808-106">Действие триггера в клиенте Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="33808-106">Trigger action on ConfigurationManager client</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33808-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33808-107">Prerequisites</span></span>
<span data-ttu-id="33808-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33808-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33808-110">Permission type</span></span>|<span data-ttu-id="33808-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33808-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33808-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="33808-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="33808-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33808-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33808-115">Not supported.</span></span>|
|<span data-ttu-id="33808-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="33808-116">Application</span></span>|<span data-ttu-id="33808-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="33808-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33808-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
```

## <a name="request-headers"></a><span data-ttu-id="33808-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33808-119">Request headers</span></span>
|<span data-ttu-id="33808-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33808-120">Header</span></span>|<span data-ttu-id="33808-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33808-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33808-122">Authorization</span></span>|<span data-ttu-id="33808-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33808-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33808-124">Accept</span></span>|<span data-ttu-id="33808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33808-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33808-126">Request body</span></span>
<span data-ttu-id="33808-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33808-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="33808-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="33808-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="33808-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33808-129">Property</span></span>|<span data-ttu-id="33808-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33808-130">Type</span></span>|<span data-ttu-id="33808-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33808-132">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="33808-132">configurationManagerAction</span></span>|[<span data-ttu-id="33808-133">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="33808-133">configurationManagerAction</span></span>](../resources/intune-devices-configurationmanageraction.md)|<span data-ttu-id="33808-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="33808-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="33808-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="33808-135">Response</span></span>
<span data-ttu-id="33808-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="33808-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="33808-137">Пример</span><span class="sxs-lookup"><span data-stu-id="33808-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="33808-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="33808-138">Request</span></span>
<span data-ttu-id="33808-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33808-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction

Content-type: application/json
Content-length: 145

{
  "configurationManagerAction": {
    "@odata.type": "microsoft.graph.configurationManagerAction",
    "action": "refreshUserPolicy"
  }
}
```

### <a name="response"></a><span data-ttu-id="33808-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="33808-140">Response</span></span>
<span data-ttu-id="33808-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






