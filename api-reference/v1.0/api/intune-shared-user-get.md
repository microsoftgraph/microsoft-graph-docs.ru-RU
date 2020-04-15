---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45c045f4088b72c5eb3ea1aeb37c086a7257079d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411353"
---
# <a name="get-user"></a><span data-ttu-id="7e785-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="7e785-103">Get user</span></span>

<span data-ttu-id="7e785-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e785-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e785-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e785-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e785-106">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7e785-106">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e785-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e785-107">Prerequisites</span></span>
<span data-ttu-id="7e785-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="7e785-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7e785-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e785-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7e785-110">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="7e785-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="7e785-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e785-111">Permission type</span></span>|<span data-ttu-id="7e785-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e785-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e785-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e785-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7e785-114">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="7e785-114">_varies by context_</span></span>|
| <span data-ttu-id="7e785-115">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="7e785-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="7e785-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e785-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7e785-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="7e785-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7e785-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e785-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7e785-119">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="7e785-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="7e785-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e785-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7e785-121">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="7e785-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7e785-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e785-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="7e785-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e785-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e785-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e785-124">Not supported.</span></span>|
|<span data-ttu-id="7e785-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e785-125">Application</span></span>|<span data-ttu-id="7e785-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e785-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e785-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e785-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e785-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e785-128">Optional query parameters</span></span>
<span data-ttu-id="7e785-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e785-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7e785-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e785-130">Request headers</span></span>
|<span data-ttu-id="7e785-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e785-131">Header</span></span>|<span data-ttu-id="7e785-132">Значение</span><span class="sxs-lookup"><span data-stu-id="7e785-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e785-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e785-133">Authorization</span></span>|<span data-ttu-id="7e785-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e785-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e785-135">Accept</span><span class="sxs-lookup"><span data-stu-id="7e785-135">Accept</span></span>|<span data-ttu-id="7e785-136">application/json</span><span class="sxs-lookup"><span data-stu-id="7e785-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e785-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e785-137">Request body</span></span>
<span data-ttu-id="7e785-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e785-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e785-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e785-139">Response</span></span>
<span data-ttu-id="7e785-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e785-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e785-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7e785-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e785-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e785-142">Request</span></span>
<span data-ttu-id="7e785-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e785-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="7e785-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e785-144">Response</span></span>
<span data-ttu-id="7e785-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e785-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```






