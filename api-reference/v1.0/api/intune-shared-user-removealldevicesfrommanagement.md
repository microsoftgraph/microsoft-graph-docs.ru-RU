---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9c2d962fad26624d4ef82c8f68959a27cfccd6b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361247"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="a98c0-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="a98c0-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="a98c0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a98c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a98c0-105">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="a98c0-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a98c0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a98c0-106">Prerequisites</span></span>
<span data-ttu-id="a98c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a98c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a98c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a98c0-109">Permission type</span></span>|<span data-ttu-id="a98c0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a98c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a98c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a98c0-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a98c0-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="a98c0-112">_varies by context_</span></span> |
| <span data-ttu-id="a98c0-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="a98c0-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="a98c0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a98c0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="a98c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a98c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a98c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a98c0-116">Not supported.</span></span>|
|<span data-ttu-id="a98c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a98c0-117">Application</span></span>|<span data-ttu-id="a98c0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a98c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a98c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a98c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="a98c0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a98c0-120">Request headers</span></span>
|<span data-ttu-id="a98c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a98c0-121">Header</span></span>|<span data-ttu-id="a98c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a98c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a98c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a98c0-123">Authorization</span></span>|<span data-ttu-id="a98c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a98c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a98c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a98c0-125">Accept</span></span>|<span data-ttu-id="a98c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a98c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a98c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a98c0-127">Request body</span></span>
<span data-ttu-id="a98c0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a98c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a98c0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a98c0-129">Response</span></span>
<span data-ttu-id="a98c0-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a98c0-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a98c0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a98c0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a98c0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a98c0-132">Request</span></span>
<span data-ttu-id="a98c0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a98c0-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="a98c0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a98c0-134">Response</span></span>
<span data-ttu-id="a98c0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a98c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




