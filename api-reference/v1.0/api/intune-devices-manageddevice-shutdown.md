---
title: Действие shutDown
description: Завершение работы устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a58ec2237994a49f51fb3eaa301257d2ea883207
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364300"
---
# <a name="shutdown-action"></a><span data-ttu-id="76838-103">Действие shutDown</span><span class="sxs-lookup"><span data-stu-id="76838-103">shutDown action</span></span>

> <span data-ttu-id="76838-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76838-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76838-105">Завершение работы устройства</span><span class="sxs-lookup"><span data-stu-id="76838-105">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76838-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76838-106">Prerequisites</span></span>
<span data-ttu-id="76838-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76838-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76838-109">Permission type</span></span>|<span data-ttu-id="76838-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76838-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76838-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76838-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76838-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="76838-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="76838-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76838-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76838-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76838-114">Not supported.</span></span>|
|<span data-ttu-id="76838-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76838-115">Application</span></span>|<span data-ttu-id="76838-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76838-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76838-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76838-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="76838-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76838-118">Request headers</span></span>
|<span data-ttu-id="76838-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76838-119">Header</span></span>|<span data-ttu-id="76838-120">Значение</span><span class="sxs-lookup"><span data-stu-id="76838-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76838-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76838-121">Authorization</span></span>|<span data-ttu-id="76838-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76838-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76838-123">Accept</span><span class="sxs-lookup"><span data-stu-id="76838-123">Accept</span></span>|<span data-ttu-id="76838-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76838-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76838-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76838-125">Request body</span></span>
<span data-ttu-id="76838-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76838-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76838-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="76838-127">Response</span></span>
<span data-ttu-id="76838-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76838-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76838-129">Пример</span><span class="sxs-lookup"><span data-stu-id="76838-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="76838-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="76838-130">Request</span></span>
<span data-ttu-id="76838-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76838-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="76838-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="76838-132">Response</span></span>
<span data-ttu-id="76838-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76838-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




