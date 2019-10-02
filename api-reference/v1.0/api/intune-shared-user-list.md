---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae9469fca1f64b02d3e6555d9845b6270dcb6359
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361268"
---
# <a name="list-users"></a><span data-ttu-id="79306-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="79306-103">List users</span></span>

> <span data-ttu-id="79306-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79306-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79306-105">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="79306-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79306-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79306-106">Prerequisites</span></span>
<span data-ttu-id="79306-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="79306-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="79306-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79306-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="79306-109">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="79306-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="79306-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79306-110">Permission type</span></span>|<span data-ttu-id="79306-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79306-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79306-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79306-112">Delegated (work or school account)</span></span>| <span data-ttu-id="79306-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="79306-113">_varies by context_</span></span>|
| <span data-ttu-id="79306-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="79306-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="79306-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="79306-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="79306-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="79306-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="79306-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79306-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="79306-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="79306-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="79306-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79306-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="79306-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="79306-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="79306-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="79306-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="79306-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79306-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79306-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79306-123">Not supported.</span></span>|
|<span data-ttu-id="79306-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79306-124">Application</span></span>|<span data-ttu-id="79306-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79306-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79306-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79306-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="79306-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79306-127">Request headers</span></span>
|<span data-ttu-id="79306-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79306-128">Header</span></span>|<span data-ttu-id="79306-129">Значение</span><span class="sxs-lookup"><span data-stu-id="79306-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79306-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79306-130">Authorization</span></span>|<span data-ttu-id="79306-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79306-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79306-132">Accept</span><span class="sxs-lookup"><span data-stu-id="79306-132">Accept</span></span>|<span data-ttu-id="79306-133">application/json</span><span class="sxs-lookup"><span data-stu-id="79306-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79306-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79306-134">Request body</span></span>
<span data-ttu-id="79306-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79306-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79306-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="79306-136">Response</span></span>
<span data-ttu-id="79306-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79306-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79306-138">Пример</span><span class="sxs-lookup"><span data-stu-id="79306-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="79306-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="79306-139">Request</span></span>
<span data-ttu-id="79306-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79306-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="79306-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="79306-141">Response</span></span>
<span data-ttu-id="79306-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79306-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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




