---
title: Действие removeAllDevicesFromManagement
description: Прекращение управления всеми устройствами для этого пользователя
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40baa470968c10bbe26af1d8397306f5b9e3f736
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576656"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="c7349-103">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="c7349-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="c7349-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7349-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7349-105">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="c7349-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7349-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7349-106">Prerequisites</span></span>
<span data-ttu-id="c7349-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7349-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7349-109">Permission type</span></span>|<span data-ttu-id="c7349-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7349-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7349-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7349-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c7349-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="c7349-112">_varies by context_</span></span> |
| <span data-ttu-id="c7349-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="c7349-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="c7349-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c7349-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="c7349-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7349-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7349-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7349-116">Not supported.</span></span>|
|<span data-ttu-id="c7349-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7349-117">Application</span></span>|<span data-ttu-id="c7349-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7349-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7349-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7349-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="c7349-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7349-120">Request headers</span></span>
|<span data-ttu-id="c7349-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7349-121">Header</span></span>|<span data-ttu-id="c7349-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7349-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7349-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7349-123">Authorization</span></span>|<span data-ttu-id="c7349-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7349-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7349-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7349-125">Accept</span></span>|<span data-ttu-id="c7349-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7349-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7349-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7349-127">Request body</span></span>
<span data-ttu-id="c7349-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7349-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7349-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7349-129">Response</span></span>
<span data-ttu-id="c7349-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7349-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7349-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7349-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7349-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7349-132">Request</span></span>
<span data-ttu-id="c7349-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7349-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="c7349-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7349-134">Response</span></span>
<span data-ttu-id="c7349-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7349-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



