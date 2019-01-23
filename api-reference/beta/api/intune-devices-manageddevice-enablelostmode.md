---
title: Действие enableLostMode
description: Включение режима потеряны
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16a6bb61605272cc6412e788ae9a4af7a9e8340d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412620"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="9c7b3-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="9c7b3-103">enableLostMode action</span></span>

> <span data-ttu-id="9c7b3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c7b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c7b3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c7b3-107">Включение режима потеряны</span><span class="sxs-lookup"><span data-stu-id="9c7b3-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c7b3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9c7b3-108">Prerequisites</span></span>
<span data-ttu-id="9c7b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c7b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9c7b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c7b3-111">Permission type</span></span>|<span data-ttu-id="9c7b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c7b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c7b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c7b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c7b3-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9c7b3-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9c7b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c7b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c7b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-116">Not supported.</span></span>|
|<span data-ttu-id="9c7b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c7b3-117">Application</span></span>|<span data-ttu-id="9c7b3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c7b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c7b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="9c7b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c7b3-120">Request headers</span></span>
|<span data-ttu-id="9c7b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c7b3-121">Header</span></span>|<span data-ttu-id="9c7b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c7b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c7b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7b3-123">Authorization</span></span>|<span data-ttu-id="9c7b3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9c7b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c7b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c7b3-125">Accept</span></span>|<span data-ttu-id="9c7b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c7b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c7b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c7b3-127">Request body</span></span>
<span data-ttu-id="9c7b3-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9c7b3-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9c7b3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c7b3-130">Property</span></span>|<span data-ttu-id="9c7b3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9c7b3-131">Type</span></span>|<span data-ttu-id="9c7b3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9c7b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c7b3-133">message</span><span class="sxs-lookup"><span data-stu-id="9c7b3-133">message</span></span>|<span data-ttu-id="9c7b3-134">String</span><span class="sxs-lookup"><span data-stu-id="9c7b3-134">String</span></span>|<span data-ttu-id="9c7b3-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9c7b3-135">Not yet documented</span></span>|
|<span data-ttu-id="9c7b3-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9c7b3-136">phoneNumber</span></span>|<span data-ttu-id="9c7b3-137">String</span><span class="sxs-lookup"><span data-stu-id="9c7b3-137">String</span></span>|<span data-ttu-id="9c7b3-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9c7b3-138">Not yet documented</span></span>|
|<span data-ttu-id="9c7b3-139">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="9c7b3-139">footer</span></span>|<span data-ttu-id="9c7b3-140">String</span><span class="sxs-lookup"><span data-stu-id="9c7b3-140">String</span></span>|<span data-ttu-id="9c7b3-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9c7b3-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c7b3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c7b3-142">Response</span></span>
<span data-ttu-id="9c7b3-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c7b3-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9c7b3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c7b3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c7b3-145">Request</span></span>
<span data-ttu-id="9c7b3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="9c7b3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c7b3-147">Response</span></span>
<span data-ttu-id="9c7b3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c7b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




