---
title: Действие shutDown
description: Завершение работы устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1788c0c77d80eb1b1735a39767b9c335deb8053
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753563"
---
# <a name="shutdown-action"></a><span data-ttu-id="54886-103">Действие shutDown</span><span class="sxs-lookup"><span data-stu-id="54886-103">shutDown action</span></span>

<span data-ttu-id="54886-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54886-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54886-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54886-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54886-106">Завершение работы устройства</span><span class="sxs-lookup"><span data-stu-id="54886-106">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54886-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="54886-107">Prerequisites</span></span>
<span data-ttu-id="54886-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54886-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54886-110">Permission type</span></span>|<span data-ttu-id="54886-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54886-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54886-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54886-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54886-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="54886-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="54886-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54886-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54886-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54886-115">Not supported.</span></span>|
|<span data-ttu-id="54886-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="54886-116">Application</span></span>|<span data-ttu-id="54886-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="54886-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54886-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54886-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="54886-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="54886-119">Request headers</span></span>
|<span data-ttu-id="54886-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54886-120">Header</span></span>|<span data-ttu-id="54886-121">Значение</span><span class="sxs-lookup"><span data-stu-id="54886-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54886-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54886-122">Authorization</span></span>|<span data-ttu-id="54886-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54886-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54886-124">Accept</span><span class="sxs-lookup"><span data-stu-id="54886-124">Accept</span></span>|<span data-ttu-id="54886-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54886-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54886-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54886-126">Request body</span></span>
<span data-ttu-id="54886-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54886-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54886-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="54886-128">Response</span></span>
<span data-ttu-id="54886-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="54886-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54886-130">Пример</span><span class="sxs-lookup"><span data-stu-id="54886-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="54886-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="54886-131">Request</span></span>
<span data-ttu-id="54886-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54886-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="54886-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="54886-133">Response</span></span>
<span data-ttu-id="54886-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54886-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




