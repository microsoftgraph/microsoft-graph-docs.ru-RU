---
title: Действие unassignResourceAccountFromDevice
description: Отменяет назначение учетной записи ресурса для автопилотного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03f1dc44b3491e563972a7d3b4950c608f8d8020
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995491"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="18a85-103">Действие unassignResourceAccountFromDevice</span><span class="sxs-lookup"><span data-stu-id="18a85-103">unassignResourceAccountFromDevice action</span></span>

> <span data-ttu-id="18a85-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a85-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18a85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a85-106">Отменяет назначение учетной записи ресурса для автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="18a85-106">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a85-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18a85-107">Prerequisites</span></span>
<span data-ttu-id="18a85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18a85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18a85-110">Permission type</span></span>|<span data-ttu-id="18a85-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18a85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18a85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18a85-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a85-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18a85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18a85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a85-115">Not supported.</span></span>|
|<span data-ttu-id="18a85-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18a85-116">Application</span></span>|<span data-ttu-id="18a85-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a85-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18a85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="18a85-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18a85-119">Request headers</span></span>
|<span data-ttu-id="18a85-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18a85-120">Header</span></span>|<span data-ttu-id="18a85-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18a85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a85-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18a85-122">Authorization</span></span>|<span data-ttu-id="18a85-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18a85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a85-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18a85-124">Accept</span></span>|<span data-ttu-id="18a85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18a85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a85-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18a85-126">Request body</span></span>
<span data-ttu-id="18a85-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18a85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18a85-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="18a85-128">Response</span></span>
<span data-ttu-id="18a85-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18a85-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18a85-130">Пример</span><span class="sxs-lookup"><span data-stu-id="18a85-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a85-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="18a85-131">Request</span></span>
<span data-ttu-id="18a85-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18a85-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="18a85-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18a85-133">Response</span></span>
<span data-ttu-id="18a85-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18a85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





