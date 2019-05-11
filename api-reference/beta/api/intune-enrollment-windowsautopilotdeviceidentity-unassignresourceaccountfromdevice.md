---
title: Действие unassignResourceAccountFromDevice
description: Отменяет назначение учетной записи ресурса для автопилотного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe71d4112a7b4a764ee466f50ca6598245a5b66c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908160"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="3e252-103">Действие unassignResourceAccountFromDevice</span><span class="sxs-lookup"><span data-stu-id="3e252-103">unassignResourceAccountFromDevice action</span></span>

> <span data-ttu-id="3e252-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e252-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e252-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e252-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e252-106">Отменяет назначение учетной записи ресурса для автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="3e252-106">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e252-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e252-107">Prerequisites</span></span>
<span data-ttu-id="3e252-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e252-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e252-110">Permission type</span></span>|<span data-ttu-id="3e252-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e252-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e252-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e252-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e252-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e252-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e252-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e252-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e252-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e252-115">Not supported.</span></span>|
|<span data-ttu-id="3e252-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e252-116">Application</span></span>|<span data-ttu-id="3e252-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e252-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e252-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e252-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="3e252-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e252-119">Request headers</span></span>
|<span data-ttu-id="3e252-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e252-120">Header</span></span>|<span data-ttu-id="3e252-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e252-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e252-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e252-122">Authorization</span></span>|<span data-ttu-id="3e252-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e252-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e252-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e252-124">Accept</span></span>|<span data-ttu-id="3e252-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e252-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e252-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e252-126">Request body</span></span>
<span data-ttu-id="3e252-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e252-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e252-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e252-128">Response</span></span>
<span data-ttu-id="3e252-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e252-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e252-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3e252-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e252-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e252-131">Request</span></span>
<span data-ttu-id="3e252-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e252-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="3e252-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e252-133">Response</span></span>
<span data-ttu-id="3e252-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e252-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




