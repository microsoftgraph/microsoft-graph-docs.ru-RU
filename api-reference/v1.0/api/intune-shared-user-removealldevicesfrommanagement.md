---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2072d8022aa95c82dcdc6deae727c4fd7f64b7fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038503"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="4bd15-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="4bd15-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="4bd15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bd15-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bd15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bd15-106">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="4bd15-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bd15-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4bd15-107">Prerequisites</span></span>
<span data-ttu-id="4bd15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd15-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd15-110">Permission type</span></span>|<span data-ttu-id="4bd15-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bd15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bd15-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bd15-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4bd15-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="4bd15-113">_varies by context_</span></span> |
| <span data-ttu-id="4bd15-114">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="4bd15-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="4bd15-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4bd15-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="4bd15-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bd15-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bd15-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd15-117">Not supported.</span></span>|
|<span data-ttu-id="4bd15-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bd15-118">Application</span></span>|<span data-ttu-id="4bd15-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd15-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bd15-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bd15-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="4bd15-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bd15-121">Request headers</span></span>
|<span data-ttu-id="4bd15-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bd15-122">Header</span></span>|<span data-ttu-id="4bd15-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4bd15-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bd15-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd15-124">Authorization</span></span>|<span data-ttu-id="4bd15-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bd15-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bd15-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4bd15-126">Accept</span></span>|<span data-ttu-id="4bd15-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4bd15-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd15-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bd15-128">Request body</span></span>
<span data-ttu-id="4bd15-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bd15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bd15-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd15-130">Response</span></span>
<span data-ttu-id="4bd15-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4bd15-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4bd15-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4bd15-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bd15-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bd15-133">Request</span></span>
<span data-ttu-id="4bd15-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bd15-134">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="4bd15-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd15-135">Response</span></span>
<span data-ttu-id="4bd15-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bd15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









