---
title: Действие assignUserToDevice
description: Назначает пользователя устройствам автопилота.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 377cd1d1323a4f9973c49d4fb1c9a8b8ebd62616
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753395"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="2001c-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="2001c-103">assignUserToDevice action</span></span>

<span data-ttu-id="2001c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2001c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2001c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2001c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2001c-106">Назначает пользователя устройствам автопилота.</span><span class="sxs-lookup"><span data-stu-id="2001c-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2001c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2001c-107">Prerequisites</span></span>
<span data-ttu-id="2001c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2001c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2001c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2001c-110">Permission type</span></span>|<span data-ttu-id="2001c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2001c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2001c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2001c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2001c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2001c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2001c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2001c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2001c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2001c-115">Not supported.</span></span>|
|<span data-ttu-id="2001c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2001c-116">Application</span></span>|<span data-ttu-id="2001c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2001c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2001c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2001c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="2001c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2001c-119">Request headers</span></span>
|<span data-ttu-id="2001c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2001c-120">Header</span></span>|<span data-ttu-id="2001c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2001c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2001c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2001c-122">Authorization</span></span>|<span data-ttu-id="2001c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2001c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2001c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2001c-124">Accept</span></span>|<span data-ttu-id="2001c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2001c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2001c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2001c-126">Request body</span></span>
<span data-ttu-id="2001c-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2001c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2001c-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2001c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2001c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2001c-129">Property</span></span>|<span data-ttu-id="2001c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2001c-130">Type</span></span>|<span data-ttu-id="2001c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2001c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2001c-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2001c-132">userPrincipalName</span></span>|<span data-ttu-id="2001c-133">String</span><span class="sxs-lookup"><span data-stu-id="2001c-133">String</span></span>|<span data-ttu-id="2001c-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2001c-134">Not yet documented</span></span>|
|<span data-ttu-id="2001c-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="2001c-135">addressableUserName</span></span>|<span data-ttu-id="2001c-136">String</span><span class="sxs-lookup"><span data-stu-id="2001c-136">String</span></span>|<span data-ttu-id="2001c-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2001c-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2001c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="2001c-138">Response</span></span>
<span data-ttu-id="2001c-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2001c-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2001c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2001c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2001c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2001c-141">Request</span></span>
<span data-ttu-id="2001c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2001c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="2001c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2001c-143">Response</span></span>
<span data-ttu-id="2001c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2001c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




