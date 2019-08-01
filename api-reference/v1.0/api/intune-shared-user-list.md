---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97575c3d323641fa0a4f86f92bb8290ad0d7c815
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025787"
---
# <a name="list-users"></a><span data-ttu-id="9d42c-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="9d42c-103">List users</span></span>

> <span data-ttu-id="9d42c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d42c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d42c-105">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="9d42c-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d42c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d42c-106">Prerequisites</span></span>
<span data-ttu-id="9d42c-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="9d42c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9d42c-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d42c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9d42c-109">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="9d42c-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="9d42c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d42c-110">Permission type</span></span>|<span data-ttu-id="9d42c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d42c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d42c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d42c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9d42c-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="9d42c-113">_varies by context_</span></span>|
| <span data-ttu-id="9d42c-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="9d42c-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9d42c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d42c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="9d42c-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9d42c-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="9d42c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d42c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="9d42c-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="9d42c-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9d42c-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d42c-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="9d42c-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="9d42c-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9d42c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d42c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="9d42c-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d42c-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d42c-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d42c-123">Not supported.</span></span>|
|<span data-ttu-id="9d42c-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d42c-124">Application</span></span>|<span data-ttu-id="9d42c-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d42c-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d42c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d42c-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="9d42c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d42c-127">Request headers</span></span>
|<span data-ttu-id="9d42c-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d42c-128">Header</span></span>|<span data-ttu-id="9d42c-129">Значение</span><span class="sxs-lookup"><span data-stu-id="9d42c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d42c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d42c-130">Authorization</span></span>|<span data-ttu-id="9d42c-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d42c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d42c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="9d42c-132">Accept</span></span>|<span data-ttu-id="9d42c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="9d42c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d42c-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d42c-134">Request body</span></span>
<span data-ttu-id="9d42c-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d42c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d42c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d42c-136">Response</span></span>
<span data-ttu-id="9d42c-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d42c-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d42c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9d42c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d42c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d42c-139">Request</span></span>
<span data-ttu-id="9d42c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d42c-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="9d42c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d42c-141">Response</span></span>
<span data-ttu-id="9d42c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d42c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



