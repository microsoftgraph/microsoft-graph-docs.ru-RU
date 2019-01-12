---
title: Действие unassignUserFromDevice
description: Unassigns пользователя из устройства автопилот.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a68c64f06b7d6e9c33817c55d0bbd4af5e1b29a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974632"
---
# <a name="unassignuserfromdevice-action"></a><span data-ttu-id="ab5f0-103">Действие unassignUserFromDevice</span><span class="sxs-lookup"><span data-stu-id="ab5f0-103">unassignUserFromDevice action</span></span>

> <span data-ttu-id="ab5f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab5f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab5f0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab5f0-107">Unassigns пользователя из устройства автопилот.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-107">Unassigns the user from an Autopilot device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab5f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab5f0-108">Prerequisites</span></span>
<span data-ttu-id="ab5f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab5f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab5f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5f0-111">Permission type</span></span>|<span data-ttu-id="ab5f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab5f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab5f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab5f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab5f0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab5f0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ab5f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab5f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab5f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-116">Not supported.</span></span>|
|<span data-ttu-id="ab5f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab5f0-117">Application</span></span>|<span data-ttu-id="ab5f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab5f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab5f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignUserFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignUserFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="ab5f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab5f0-120">Request headers</span></span>
|<span data-ttu-id="ab5f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab5f0-121">Header</span></span>|<span data-ttu-id="ab5f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab5f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab5f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab5f0-123">Authorization</span></span>|<span data-ttu-id="ab5f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab5f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab5f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab5f0-125">Accept</span></span>|<span data-ttu-id="ab5f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab5f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab5f0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab5f0-127">Request body</span></span>
<span data-ttu-id="ab5f0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab5f0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab5f0-129">Response</span></span>
<span data-ttu-id="ab5f0-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ab5f0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ab5f0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab5f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab5f0-132">Request</span></span>
<span data-ttu-id="ab5f0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignUserFromDevice
```

### <a name="response"></a><span data-ttu-id="ab5f0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab5f0-134">Response</span></span>
<span data-ttu-id="ab5f0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab5f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





