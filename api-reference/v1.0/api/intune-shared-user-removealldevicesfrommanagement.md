---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: tfitzmac
ms.openlocfilehash: 8d563466074075365c94ed69358f72cf24783bea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339755"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="b9012-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="b9012-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="b9012-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9012-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9012-105">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="b9012-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9012-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b9012-106">Prerequisites</span></span>
<span data-ttu-id="b9012-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9012-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9012-109">Permission type</span></span>|<span data-ttu-id="b9012-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9012-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9012-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9012-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b9012-112">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="b9012-112">_varies by context_</span></span> |
| <span data-ttu-id="b9012-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="b9012-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="b9012-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b9012-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="b9012-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9012-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9012-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9012-116">Not supported.</span></span>|
|<span data-ttu-id="b9012-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9012-117">Application</span></span>|<span data-ttu-id="b9012-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9012-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9012-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9012-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="b9012-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9012-120">Request headers</span></span>
|<span data-ttu-id="b9012-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9012-121">Header</span></span>|<span data-ttu-id="b9012-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9012-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9012-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9012-123">Authorization</span></span>|<span data-ttu-id="b9012-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b9012-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9012-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9012-125">Accept</span></span>|<span data-ttu-id="b9012-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9012-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9012-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9012-127">Request body</span></span>
<span data-ttu-id="b9012-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9012-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9012-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9012-129">Response</span></span>
<span data-ttu-id="b9012-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9012-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9012-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9012-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9012-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9012-132">Request</span></span>
<span data-ttu-id="b9012-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9012-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="b9012-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9012-134">Response</span></span>
<span data-ttu-id="b9012-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9012-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



