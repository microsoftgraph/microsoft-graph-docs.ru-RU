---
title: Действие requestRemoteAssistance
description: Запрос удаленной помощи
ms.openlocfilehash: b33b8ef0c9af355325d2d27d0db476338766c741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081071"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="7b5bc-103">Действие requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="7b5bc-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="7b5bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b5bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b5bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b5bc-107">Запрос удаленной помощи</span><span class="sxs-lookup"><span data-stu-id="7b5bc-107">Request remote assistance</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b5bc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7b5bc-108">Prerequisites</span></span>
<span data-ttu-id="7b5bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b5bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b5bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b5bc-111">Permission type</span></span>|<span data-ttu-id="7b5bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b5bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b5bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b5bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b5bc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b5bc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b5bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b5bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b5bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-116">Not supported.</span></span>|
|<span data-ttu-id="7b5bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b5bc-117">Application</span></span>|<span data-ttu-id="7b5bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b5bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b5bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="7b5bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b5bc-120">Request headers</span></span>
|<span data-ttu-id="7b5bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b5bc-121">Header</span></span>|<span data-ttu-id="7b5bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b5bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b5bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b5bc-123">Authorization</span></span>|<span data-ttu-id="7b5bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b5bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b5bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b5bc-125">Accept</span></span>|<span data-ttu-id="7b5bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b5bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b5bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b5bc-127">Request body</span></span>
<span data-ttu-id="7b5bc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b5bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b5bc-129">Response</span></span>
<span data-ttu-id="7b5bc-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b5bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7b5bc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b5bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b5bc-132">Request</span></span>
<span data-ttu-id="7b5bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b5bc-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="7b5bc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b5bc-134">Response</span></span>
<span data-ttu-id="7b5bc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7b5bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





