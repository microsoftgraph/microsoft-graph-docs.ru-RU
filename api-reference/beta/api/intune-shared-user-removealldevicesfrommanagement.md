---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30af7f1924e4a938957eb43b940c6b9eca4fe13b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800531"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="ccb3e-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="ccb3e-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="ccb3e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccb3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccb3e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccb3e-107">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="ccb3e-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ccb3e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ccb3e-108">Prerequisites</span></span>
<span data-ttu-id="ccb3e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccb3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccb3e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccb3e-111">Permission type</span></span>|<span data-ttu-id="ccb3e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccb3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccb3e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccb3e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ccb3e-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ccb3e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ccb3e-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ccb3e-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ccb3e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccb3e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccb3e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-117">Not supported.</span></span>|
|<span data-ttu-id="ccb3e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="ccb3e-118">Application</span></span>||
| <span data-ttu-id="ccb3e-119">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ccb3e-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ccb3e-120">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ccb3e-120">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccb3e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccb3e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="ccb3e-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccb3e-122">Request headers</span></span>
|<span data-ttu-id="ccb3e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccb3e-123">Header</span></span>|<span data-ttu-id="ccb3e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ccb3e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccb3e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccb3e-125">Authorization</span></span>|<span data-ttu-id="ccb3e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccb3e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ccb3e-127">Accept</span></span>|<span data-ttu-id="ccb3e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ccb3e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccb3e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccb3e-129">Request body</span></span>
<span data-ttu-id="ccb3e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccb3e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccb3e-131">Response</span></span>
<span data-ttu-id="ccb3e-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ccb3e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ccb3e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ccb3e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccb3e-134">Request</span></span>
<span data-ttu-id="ccb3e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="ccb3e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccb3e-136">Response</span></span>
<span data-ttu-id="ccb3e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccb3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












