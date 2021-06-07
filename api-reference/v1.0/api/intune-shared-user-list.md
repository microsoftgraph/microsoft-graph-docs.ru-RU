---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d06b458b96598c892dc068a13d8aadc728d28505
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732842"
---
# <a name="list-users"></a><span data-ttu-id="a91ff-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="a91ff-103">List users</span></span>

<span data-ttu-id="a91ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a91ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a91ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a91ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a91ff-106">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="a91ff-106">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a91ff-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a91ff-107">Prerequisites</span></span>
<span data-ttu-id="a91ff-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a91ff-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a91ff-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91ff-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="a91ff-110">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="a91ff-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="a91ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a91ff-111">Permission type</span></span>|<span data-ttu-id="a91ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a91ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a91ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a91ff-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a91ff-114">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="a91ff-114">_varies by context_</span></span>|
| <span data-ttu-id="a91ff-115">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="a91ff-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="a91ff-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a91ff-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="a91ff-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="a91ff-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="a91ff-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a91ff-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="a91ff-119">&nbsp;&nbsp;Onboarding</span><span class="sxs-lookup"><span data-stu-id="a91ff-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="a91ff-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a91ff-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="a91ff-121">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="a91ff-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="a91ff-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a91ff-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="a91ff-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a91ff-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a91ff-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91ff-124">Not supported.</span></span>|
|<span data-ttu-id="a91ff-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a91ff-125">Application</span></span>|<span data-ttu-id="a91ff-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91ff-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a91ff-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a91ff-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="a91ff-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a91ff-128">Request headers</span></span>
|<span data-ttu-id="a91ff-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a91ff-129">Header</span></span>|<span data-ttu-id="a91ff-130">Значение</span><span class="sxs-lookup"><span data-stu-id="a91ff-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a91ff-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91ff-131">Authorization</span></span>|<span data-ttu-id="a91ff-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91ff-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a91ff-133">Accept</span><span class="sxs-lookup"><span data-stu-id="a91ff-133">Accept</span></span>|<span data-ttu-id="a91ff-134">application/json</span><span class="sxs-lookup"><span data-stu-id="a91ff-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a91ff-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a91ff-135">Request body</span></span>
<span data-ttu-id="a91ff-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a91ff-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a91ff-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91ff-137">Response</span></span>
<span data-ttu-id="a91ff-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a91ff-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a91ff-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a91ff-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a91ff-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91ff-140">Request</span></span>
<span data-ttu-id="a91ff-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a91ff-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="a91ff-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91ff-142">Response</span></span>
<span data-ttu-id="a91ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a91ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









