---
title: Действие remoteLock
description: Удаленная блокировка
author: tfitzmac
ms.openlocfilehash: d601ad92b37bdf2b4b943588c47414373904eaee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337732"
---
# <a name="remotelock-action"></a><span data-ttu-id="cf77b-103">Действие remoteLock</span><span class="sxs-lookup"><span data-stu-id="cf77b-103">remoteLock action</span></span>

> <span data-ttu-id="cf77b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf77b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf77b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf77b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf77b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf77b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf77b-107">Удаленная блокировка</span><span class="sxs-lookup"><span data-stu-id="cf77b-107">Remote lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf77b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cf77b-108">Prerequisites</span></span>
<span data-ttu-id="cf77b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf77b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf77b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf77b-111">Permission type</span></span>|<span data-ttu-id="cf77b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf77b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf77b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf77b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf77b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cf77b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cf77b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf77b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf77b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf77b-116">Not supported.</span></span>|
|<span data-ttu-id="cf77b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf77b-117">Application</span></span>|<span data-ttu-id="cf77b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf77b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf77b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf77b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="cf77b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf77b-120">Request headers</span></span>
|<span data-ttu-id="cf77b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf77b-121">Header</span></span>|<span data-ttu-id="cf77b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf77b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf77b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf77b-123">Authorization</span></span>|<span data-ttu-id="cf77b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cf77b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf77b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf77b-125">Accept</span></span>|<span data-ttu-id="cf77b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf77b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf77b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf77b-127">Request body</span></span>
<span data-ttu-id="cf77b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf77b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf77b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf77b-129">Response</span></span>
<span data-ttu-id="cf77b-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cf77b-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf77b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf77b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf77b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf77b-132">Request</span></span>
<span data-ttu-id="cf77b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf77b-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="cf77b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf77b-134">Response</span></span>
<span data-ttu-id="cf77b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cf77b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





