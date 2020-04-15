---
title: Действие requestRemoteAssistance
description: Запрос удаленной помощи
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f71756c82c6a4f6b7bbf8d020407a2c03a7238
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450546"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="55288-103">Действие requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="55288-103">requestRemoteAssistance action</span></span>

<span data-ttu-id="55288-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55288-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55288-106">Запрос удаленной помощи</span><span class="sxs-lookup"><span data-stu-id="55288-106">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55288-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="55288-107">Prerequisites</span></span>
<span data-ttu-id="55288-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55288-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55288-110">Permission type</span></span>|<span data-ttu-id="55288-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55288-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55288-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55288-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55288-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55288-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="55288-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55288-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55288-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55288-115">Not supported.</span></span>|
|<span data-ttu-id="55288-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55288-116">Application</span></span>|<span data-ttu-id="55288-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55288-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55288-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55288-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="55288-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55288-119">Request headers</span></span>
|<span data-ttu-id="55288-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55288-120">Header</span></span>|<span data-ttu-id="55288-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55288-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55288-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55288-122">Authorization</span></span>|<span data-ttu-id="55288-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55288-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55288-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55288-124">Accept</span></span>|<span data-ttu-id="55288-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55288-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55288-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55288-126">Request body</span></span>
<span data-ttu-id="55288-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55288-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55288-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="55288-128">Response</span></span>
<span data-ttu-id="55288-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="55288-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="55288-130">Пример</span><span class="sxs-lookup"><span data-stu-id="55288-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="55288-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="55288-131">Request</span></span>
<span data-ttu-id="55288-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55288-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="55288-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="55288-133">Response</span></span>
<span data-ttu-id="55288-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55288-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






