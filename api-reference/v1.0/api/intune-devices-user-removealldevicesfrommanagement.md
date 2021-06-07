---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c92116defdc93d64f20030dcd2f88353e623ba71
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753434"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="8dfcc-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="8dfcc-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="8dfcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dfcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dfcc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dfcc-106">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="8dfcc-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dfcc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8dfcc-107">Prerequisites</span></span>
<span data-ttu-id="8dfcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dfcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dfcc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dfcc-110">Permission type</span></span>|<span data-ttu-id="8dfcc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dfcc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dfcc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dfcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8dfcc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8dfcc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="8dfcc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dfcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dfcc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-115">Not supported.</span></span>|
|<span data-ttu-id="8dfcc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dfcc-116">Application</span></span>|<span data-ttu-id="8dfcc-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8dfcc-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dfcc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dfcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="8dfcc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8dfcc-119">Request headers</span></span>
|<span data-ttu-id="8dfcc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dfcc-120">Header</span></span>|<span data-ttu-id="8dfcc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8dfcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dfcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dfcc-122">Authorization</span></span>|<span data-ttu-id="8dfcc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dfcc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8dfcc-124">Accept</span></span>|<span data-ttu-id="8dfcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8dfcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dfcc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dfcc-126">Request body</span></span>
<span data-ttu-id="8dfcc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dfcc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dfcc-128">Response</span></span>
<span data-ttu-id="8dfcc-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8dfcc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8dfcc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dfcc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dfcc-131">Request</span></span>
<span data-ttu-id="8dfcc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="8dfcc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dfcc-133">Response</span></span>
<span data-ttu-id="8dfcc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dfcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




