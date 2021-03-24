---
title: действие updateDeviceProperties
description: Обновляет свойства на устройствах автопилота.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58ff137b41ad9ec6c985e9ef23f1c6364464f7bb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142137"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="36987-103">действие updateDeviceProperties</span><span class="sxs-lookup"><span data-stu-id="36987-103">updateDeviceProperties action</span></span>

<span data-ttu-id="36987-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36987-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36987-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36987-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36987-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36987-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36987-107">Обновляет свойства на устройствах автопилота.</span><span class="sxs-lookup"><span data-stu-id="36987-107">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36987-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36987-108">Prerequisites</span></span>
<span data-ttu-id="36987-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36987-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36987-111">Permission type</span></span>|<span data-ttu-id="36987-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36987-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36987-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36987-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36987-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36987-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36987-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36987-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36987-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36987-116">Not supported.</span></span>|
|<span data-ttu-id="36987-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="36987-117">Application</span></span>|<span data-ttu-id="36987-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36987-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36987-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36987-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="36987-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36987-120">Request headers</span></span>
|<span data-ttu-id="36987-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36987-121">Header</span></span>|<span data-ttu-id="36987-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36987-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36987-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36987-123">Authorization</span></span>|<span data-ttu-id="36987-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36987-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36987-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36987-125">Accept</span></span>|<span data-ttu-id="36987-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36987-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36987-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36987-127">Request body</span></span>
<span data-ttu-id="36987-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36987-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="36987-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="36987-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="36987-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36987-130">Property</span></span>|<span data-ttu-id="36987-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36987-131">Type</span></span>|<span data-ttu-id="36987-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36987-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36987-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36987-133">userPrincipalName</span></span>|<span data-ttu-id="36987-134">String</span><span class="sxs-lookup"><span data-stu-id="36987-134">String</span></span>|<span data-ttu-id="36987-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36987-135">Not yet documented</span></span>|
|<span data-ttu-id="36987-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="36987-136">addressableUserName</span></span>|<span data-ttu-id="36987-137">String</span><span class="sxs-lookup"><span data-stu-id="36987-137">String</span></span>|<span data-ttu-id="36987-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36987-138">Not yet documented</span></span>|
|<span data-ttu-id="36987-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="36987-139">groupTag</span></span>|<span data-ttu-id="36987-140">String</span><span class="sxs-lookup"><span data-stu-id="36987-140">String</span></span>|<span data-ttu-id="36987-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36987-141">Not yet documented</span></span>|
|<span data-ttu-id="36987-142">displayName</span><span class="sxs-lookup"><span data-stu-id="36987-142">displayName</span></span>|<span data-ttu-id="36987-143">Строка</span><span class="sxs-lookup"><span data-stu-id="36987-143">String</span></span>|<span data-ttu-id="36987-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36987-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="36987-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="36987-145">Response</span></span>
<span data-ttu-id="36987-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="36987-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36987-147">Пример</span><span class="sxs-lookup"><span data-stu-id="36987-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="36987-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="36987-148">Request</span></span>
<span data-ttu-id="36987-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36987-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties

Content-type: application/json
Content-length: 187

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "groupTag": "Group Tag value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="36987-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="36987-150">Response</span></span>
<span data-ttu-id="36987-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36987-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




