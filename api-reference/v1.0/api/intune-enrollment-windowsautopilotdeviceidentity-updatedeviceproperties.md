---
title: действие updateDeviceProperties
description: Обновляет свойства на устройствах автопилота.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ecdca46463b608b3aa2cacd55c4f4cbe00afe0c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753378"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="aac8a-103">действие updateDeviceProperties</span><span class="sxs-lookup"><span data-stu-id="aac8a-103">updateDeviceProperties action</span></span>

<span data-ttu-id="aac8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aac8a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aac8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac8a-106">Обновляет свойства на устройствах автопилота.</span><span class="sxs-lookup"><span data-stu-id="aac8a-106">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac8a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aac8a-107">Prerequisites</span></span>
<span data-ttu-id="aac8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aac8a-110">Permission type</span></span>|<span data-ttu-id="aac8a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aac8a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aac8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aac8a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac8a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aac8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aac8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac8a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac8a-115">Not supported.</span></span>|
|<span data-ttu-id="aac8a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="aac8a-116">Application</span></span>|<span data-ttu-id="aac8a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac8a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aac8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="aac8a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aac8a-119">Request headers</span></span>
|<span data-ttu-id="aac8a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aac8a-120">Header</span></span>|<span data-ttu-id="aac8a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aac8a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac8a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac8a-122">Authorization</span></span>|<span data-ttu-id="aac8a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aac8a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac8a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aac8a-124">Accept</span></span>|<span data-ttu-id="aac8a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aac8a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac8a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aac8a-126">Request body</span></span>
<span data-ttu-id="aac8a-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aac8a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aac8a-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aac8a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aac8a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aac8a-129">Property</span></span>|<span data-ttu-id="aac8a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aac8a-130">Type</span></span>|<span data-ttu-id="aac8a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aac8a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac8a-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aac8a-132">userPrincipalName</span></span>|<span data-ttu-id="aac8a-133">String</span><span class="sxs-lookup"><span data-stu-id="aac8a-133">String</span></span>|<span data-ttu-id="aac8a-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aac8a-134">Not yet documented</span></span>|
|<span data-ttu-id="aac8a-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="aac8a-135">addressableUserName</span></span>|<span data-ttu-id="aac8a-136">String</span><span class="sxs-lookup"><span data-stu-id="aac8a-136">String</span></span>|<span data-ttu-id="aac8a-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aac8a-137">Not yet documented</span></span>|
|<span data-ttu-id="aac8a-138">groupTag</span><span class="sxs-lookup"><span data-stu-id="aac8a-138">groupTag</span></span>|<span data-ttu-id="aac8a-139">String</span><span class="sxs-lookup"><span data-stu-id="aac8a-139">String</span></span>|<span data-ttu-id="aac8a-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aac8a-140">Not yet documented</span></span>|
|<span data-ttu-id="aac8a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="aac8a-141">displayName</span></span>|<span data-ttu-id="aac8a-142">String</span><span class="sxs-lookup"><span data-stu-id="aac8a-142">String</span></span>|<span data-ttu-id="aac8a-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aac8a-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aac8a-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="aac8a-144">Response</span></span>
<span data-ttu-id="aac8a-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aac8a-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aac8a-146">Пример</span><span class="sxs-lookup"><span data-stu-id="aac8a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac8a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="aac8a-147">Request</span></span>
<span data-ttu-id="aac8a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aac8a-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties

Content-type: application/json
Content-length: 187

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "groupTag": "Group Tag value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="aac8a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac8a-149">Response</span></span>
<span data-ttu-id="aac8a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aac8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




