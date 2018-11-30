---
title: Действие assignUserToDevice
description: Назначает пользователю на автопилот устройства.
ms.openlocfilehash: 7e3152b4ac158714d37f5d5eb1b830a21dd3745d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077736"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="a6807-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="a6807-103">assignUserToDevice action</span></span>

> <span data-ttu-id="a6807-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6807-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6807-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6807-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6807-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6807-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6807-107">Назначает пользователю на автопилот устройства.</span><span class="sxs-lookup"><span data-stu-id="a6807-107">Assigns user to Autopilot devices.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6807-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6807-108">Prerequisites</span></span>
<span data-ttu-id="a6807-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6807-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6807-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6807-111">Permission type</span></span>|<span data-ttu-id="a6807-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6807-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6807-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6807-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6807-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6807-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6807-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6807-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6807-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6807-116">Not supported.</span></span>|
|<span data-ttu-id="a6807-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6807-117">Application</span></span>|<span data-ttu-id="a6807-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6807-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6807-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6807-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="a6807-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6807-120">Request headers</span></span>
|<span data-ttu-id="a6807-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6807-121">Header</span></span>|<span data-ttu-id="a6807-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a6807-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6807-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6807-123">Authorization</span></span>|<span data-ttu-id="a6807-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a6807-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6807-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6807-125">Accept</span></span>|<span data-ttu-id="a6807-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6807-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6807-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6807-127">Request body</span></span>
<span data-ttu-id="a6807-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6807-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a6807-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a6807-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a6807-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6807-130">Property</span></span>|<span data-ttu-id="a6807-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6807-131">Type</span></span>|<span data-ttu-id="a6807-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6807-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6807-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6807-133">userPrincipalName</span></span>|<span data-ttu-id="a6807-134">String</span><span class="sxs-lookup"><span data-stu-id="a6807-134">String</span></span>|<span data-ttu-id="a6807-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a6807-135">Not yet documented</span></span>|
|<span data-ttu-id="a6807-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="a6807-136">addressableUserName</span></span>|<span data-ttu-id="a6807-137">String</span><span class="sxs-lookup"><span data-stu-id="a6807-137">String</span></span>|<span data-ttu-id="a6807-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a6807-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6807-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6807-139">Response</span></span>
<span data-ttu-id="a6807-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6807-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6807-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a6807-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6807-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6807-142">Request</span></span>
<span data-ttu-id="a6807-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6807-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6807-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6807-144">Response</span></span>
<span data-ttu-id="a6807-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a6807-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





