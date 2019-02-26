---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40baa470968c10bbe26af1d8397306f5b9e3f736
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252800"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="8df0c-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="8df0c-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="8df0c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8df0c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df0c-105">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="8df0c-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df0c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8df0c-106">Prerequisites</span></span>
<span data-ttu-id="8df0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8df0c-109">Permission type</span></span>|<span data-ttu-id="8df0c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8df0c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8df0c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8df0c-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="8df0c-112">_varies by context_</span></span> |
| <span data-ttu-id="8df0c-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="8df0c-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="8df0c-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8df0c-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="8df0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8df0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df0c-116">Not supported.</span></span>|
|<span data-ttu-id="8df0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8df0c-117">Application</span></span>|<span data-ttu-id="8df0c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8df0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="8df0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8df0c-120">Request headers</span></span>
|<span data-ttu-id="8df0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8df0c-121">Header</span></span>|<span data-ttu-id="8df0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8df0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df0c-123">Authorization</span></span>|<span data-ttu-id="8df0c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8df0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8df0c-125">Accept</span></span>|<span data-ttu-id="8df0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8df0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8df0c-127">Request body</span></span>
<span data-ttu-id="8df0c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8df0c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df0c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df0c-129">Response</span></span>
<span data-ttu-id="8df0c-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8df0c-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8df0c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8df0c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df0c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8df0c-132">Request</span></span>
<span data-ttu-id="8df0c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8df0c-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="8df0c-134">Отклик
</span><span class="sxs-lookup"><span data-stu-id="8df0c-134">Response</span></span>
<span data-ttu-id="8df0c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8df0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



