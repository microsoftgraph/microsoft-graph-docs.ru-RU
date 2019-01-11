---
title: Действие retire
description: Прекращение использования устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e76c665cc54a2f7e148a377fa38252c3066f36f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861252"
---
# <a name="retire-action"></a><span data-ttu-id="46568-103">Действие retire</span><span class="sxs-lookup"><span data-stu-id="46568-103">retire action</span></span>

> <span data-ttu-id="46568-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46568-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46568-105">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="46568-105">Retire a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46568-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="46568-106">Prerequisites</span></span>
<span data-ttu-id="46568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46568-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46568-109">Permission type</span></span>|<span data-ttu-id="46568-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46568-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46568-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46568-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46568-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="46568-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="46568-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46568-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46568-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46568-114">Not supported.</span></span>|
|<span data-ttu-id="46568-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46568-115">Application</span></span>|<span data-ttu-id="46568-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46568-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46568-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46568-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/retire
```

## <a name="request-headers"></a><span data-ttu-id="46568-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46568-118">Request headers</span></span>
|<span data-ttu-id="46568-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46568-119">Header</span></span>|<span data-ttu-id="46568-120">Значение</span><span class="sxs-lookup"><span data-stu-id="46568-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46568-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46568-121">Authorization</span></span>|<span data-ttu-id="46568-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46568-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46568-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46568-123">Accept</span></span>|<span data-ttu-id="46568-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46568-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46568-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46568-125">Request body</span></span>
<span data-ttu-id="46568-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46568-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46568-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="46568-127">Response</span></span>
<span data-ttu-id="46568-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46568-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46568-129">Пример</span><span class="sxs-lookup"><span data-stu-id="46568-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="46568-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="46568-130">Request</span></span>
<span data-ttu-id="46568-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46568-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/retire
```

### <a name="response"></a><span data-ttu-id="46568-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="46568-132">Response</span></span>
<span data-ttu-id="46568-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



