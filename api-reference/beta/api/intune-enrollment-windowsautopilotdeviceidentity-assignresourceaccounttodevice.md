---
title: Действие assignResourceAccountToDevice
description: Назначение учетной записи ресурса автопилотным устройствам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7421cbc03b43af03a0d94ae5b9311540207e5d7b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982849"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="b793d-103">Действие assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="b793d-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="b793d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b793d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b793d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b793d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b793d-106">Назначение учетной записи ресурса автопилотным устройствам.</span><span class="sxs-lookup"><span data-stu-id="b793d-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b793d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b793d-107">Prerequisites</span></span>
<span data-ttu-id="b793d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b793d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b793d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b793d-110">Permission type</span></span>|<span data-ttu-id="b793d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b793d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b793d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b793d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b793d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b793d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b793d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b793d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b793d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b793d-115">Not supported.</span></span>|
|<span data-ttu-id="b793d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b793d-116">Application</span></span>|<span data-ttu-id="b793d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b793d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b793d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b793d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="b793d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b793d-119">Request headers</span></span>
|<span data-ttu-id="b793d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b793d-120">Header</span></span>|<span data-ttu-id="b793d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b793d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b793d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b793d-122">Authorization</span></span>|<span data-ttu-id="b793d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b793d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b793d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b793d-124">Accept</span></span>|<span data-ttu-id="b793d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b793d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b793d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b793d-126">Request body</span></span>
<span data-ttu-id="b793d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b793d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b793d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b793d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b793d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b793d-129">Property</span></span>|<span data-ttu-id="b793d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b793d-130">Type</span></span>|<span data-ttu-id="b793d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b793d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b793d-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b793d-132">userPrincipalName</span></span>|<span data-ttu-id="b793d-133">String</span><span class="sxs-lookup"><span data-stu-id="b793d-133">String</span></span>|<span data-ttu-id="b793d-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b793d-134">Not yet documented</span></span>|
|<span data-ttu-id="b793d-135">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="b793d-135">addressableUserName</span></span>|<span data-ttu-id="b793d-136">String</span><span class="sxs-lookup"><span data-stu-id="b793d-136">String</span></span>|<span data-ttu-id="b793d-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b793d-137">Not yet documented</span></span>|
|<span data-ttu-id="b793d-138">Ресаурцеаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="b793d-138">resourceAccountName</span></span>|<span data-ttu-id="b793d-139">String</span><span class="sxs-lookup"><span data-stu-id="b793d-139">String</span></span>|<span data-ttu-id="b793d-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b793d-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b793d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b793d-141">Response</span></span>
<span data-ttu-id="b793d-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b793d-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b793d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b793d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b793d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b793d-144">Request</span></span>
<span data-ttu-id="b793d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b793d-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="b793d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b793d-146">Response</span></span>
<span data-ttu-id="b793d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b793d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





