---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2072d8022aa95c82dcdc6deae727c4fd7f64b7fd
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732985"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="9efcc-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="9efcc-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="9efcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9efcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9efcc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9efcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9efcc-106">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="9efcc-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9efcc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9efcc-107">Prerequisites</span></span>
<span data-ttu-id="9efcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9efcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9efcc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9efcc-110">Permission type</span></span>|<span data-ttu-id="9efcc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9efcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9efcc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9efcc-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9efcc-113">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="9efcc-113">_varies by context_</span></span> |
| <span data-ttu-id="9efcc-114">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="9efcc-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9efcc-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9efcc-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="9efcc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9efcc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9efcc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9efcc-117">Not supported.</span></span>|
|<span data-ttu-id="9efcc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9efcc-118">Application</span></span>|<span data-ttu-id="9efcc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9efcc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9efcc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9efcc-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="9efcc-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9efcc-121">Request headers</span></span>
|<span data-ttu-id="9efcc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9efcc-122">Header</span></span>|<span data-ttu-id="9efcc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9efcc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9efcc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9efcc-124">Authorization</span></span>|<span data-ttu-id="9efcc-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9efcc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9efcc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9efcc-126">Accept</span></span>|<span data-ttu-id="9efcc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9efcc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9efcc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9efcc-128">Request body</span></span>
<span data-ttu-id="9efcc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9efcc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9efcc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9efcc-130">Response</span></span>
<span data-ttu-id="9efcc-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9efcc-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9efcc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9efcc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9efcc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9efcc-133">Request</span></span>
<span data-ttu-id="9efcc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9efcc-134">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="9efcc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9efcc-135">Response</span></span>
<span data-ttu-id="9efcc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9efcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









