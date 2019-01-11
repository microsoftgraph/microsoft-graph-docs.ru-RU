---
title: Действие assignUserToDevice
description: Назначает пользователю на автопилот устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33145d5852d80eef529cc58e34524c170bba62cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859460"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="beace-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="beace-103">assignUserToDevice action</span></span>

> <span data-ttu-id="beace-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="beace-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beace-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beace-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="beace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beace-107">Назначает пользователю на автопилот устройства.</span><span class="sxs-lookup"><span data-stu-id="beace-107">Assigns user to Autopilot devices.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beace-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="beace-108">Prerequisites</span></span>
<span data-ttu-id="beace-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beace-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beace-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beace-111">Permission type</span></span>|<span data-ttu-id="beace-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="beace-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beace-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beace-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beace-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beace-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="beace-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beace-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beace-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beace-116">Not supported.</span></span>|
|<span data-ttu-id="beace-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beace-117">Application</span></span>|<span data-ttu-id="beace-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beace-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beace-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beace-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="beace-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beace-120">Request headers</span></span>
|<span data-ttu-id="beace-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beace-121">Header</span></span>|<span data-ttu-id="beace-122">Значение</span><span class="sxs-lookup"><span data-stu-id="beace-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beace-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="beace-123">Authorization</span></span>|<span data-ttu-id="beace-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="beace-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beace-125">Accept</span><span class="sxs-lookup"><span data-stu-id="beace-125">Accept</span></span>|<span data-ttu-id="beace-126">application/json</span><span class="sxs-lookup"><span data-stu-id="beace-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beace-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="beace-127">Request body</span></span>
<span data-ttu-id="beace-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beace-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="beace-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="beace-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="beace-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="beace-130">Property</span></span>|<span data-ttu-id="beace-131">Тип</span><span class="sxs-lookup"><span data-stu-id="beace-131">Type</span></span>|<span data-ttu-id="beace-132">Описание</span><span class="sxs-lookup"><span data-stu-id="beace-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beace-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="beace-133">userPrincipalName</span></span>|<span data-ttu-id="beace-134">Строка</span><span class="sxs-lookup"><span data-stu-id="beace-134">String</span></span>|<span data-ttu-id="beace-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="beace-135">Not yet documented</span></span>|
|<span data-ttu-id="beace-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="beace-136">addressableUserName</span></span>|<span data-ttu-id="beace-137">Строка</span><span class="sxs-lookup"><span data-stu-id="beace-137">String</span></span>|<span data-ttu-id="beace-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="beace-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="beace-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="beace-139">Response</span></span>
<span data-ttu-id="beace-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="beace-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="beace-141">Пример</span><span class="sxs-lookup"><span data-stu-id="beace-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="beace-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="beace-142">Request</span></span>
<span data-ttu-id="beace-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beace-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="beace-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="beace-144">Response</span></span>
<span data-ttu-id="beace-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="beace-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





