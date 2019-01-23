---
title: Действие windowsDefenderUpdateSignatures
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 644adf0831907b29094c743b383b2656cbb45b5d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400433"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="377f6-103">Действие windowsDefenderUpdateSignatures</span><span class="sxs-lookup"><span data-stu-id="377f6-103">windowsDefenderUpdateSignatures action</span></span>

> <span data-ttu-id="377f6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="377f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="377f6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="377f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="377f6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="377f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="377f6-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="377f6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="377f6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="377f6-108">Prerequisites</span></span>
<span data-ttu-id="377f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="377f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="377f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="377f6-111">Permission type</span></span>|<span data-ttu-id="377f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="377f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="377f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="377f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="377f6-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="377f6-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="377f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="377f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="377f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="377f6-116">Not supported.</span></span>|
|<span data-ttu-id="377f6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="377f6-117">Application</span></span>|<span data-ttu-id="377f6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="377f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="377f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="377f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="377f6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="377f6-120">Request headers</span></span>
|<span data-ttu-id="377f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="377f6-121">Header</span></span>|<span data-ttu-id="377f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="377f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="377f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="377f6-123">Authorization</span></span>|<span data-ttu-id="377f6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="377f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="377f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="377f6-125">Accept</span></span>|<span data-ttu-id="377f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="377f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="377f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="377f6-127">Request body</span></span>
<span data-ttu-id="377f6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="377f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="377f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="377f6-129">Response</span></span>
<span data-ttu-id="377f6-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="377f6-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="377f6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="377f6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="377f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="377f6-132">Request</span></span>
<span data-ttu-id="377f6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="377f6-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="377f6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="377f6-134">Response</span></span>
<span data-ttu-id="377f6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="377f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




