---
title: Действие requestRemoteAssistance
description: Запрос удаленной помощи
author: tfitzmac
ms.openlocfilehash: 30d84f939fbd7d411bce21eca284d951f4c5cd43
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321485"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="0f135-103">Действие requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="0f135-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="0f135-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f135-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f135-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f135-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f135-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f135-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f135-107">Запрос удаленной помощи</span><span class="sxs-lookup"><span data-stu-id="0f135-107">Request remote assistance</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f135-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0f135-108">Prerequisites</span></span>
<span data-ttu-id="0f135-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f135-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f135-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f135-111">Permission type</span></span>|<span data-ttu-id="0f135-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f135-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f135-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f135-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f135-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f135-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f135-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f135-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f135-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f135-116">Not supported.</span></span>|
|<span data-ttu-id="0f135-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f135-117">Application</span></span>|<span data-ttu-id="0f135-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f135-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f135-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f135-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0f135-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f135-120">Request headers</span></span>
|<span data-ttu-id="0f135-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f135-121">Header</span></span>|<span data-ttu-id="0f135-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f135-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f135-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f135-123">Authorization</span></span>|<span data-ttu-id="0f135-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0f135-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f135-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f135-125">Accept</span></span>|<span data-ttu-id="0f135-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f135-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f135-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f135-127">Request body</span></span>
<span data-ttu-id="0f135-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f135-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f135-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f135-129">Response</span></span>
<span data-ttu-id="0f135-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f135-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f135-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0f135-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f135-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f135-132">Request</span></span>
<span data-ttu-id="0f135-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f135-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="0f135-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f135-134">Response</span></span>
<span data-ttu-id="0f135-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0f135-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





