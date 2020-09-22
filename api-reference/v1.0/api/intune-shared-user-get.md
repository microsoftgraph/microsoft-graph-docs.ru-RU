---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c101ae6f807f6dba76b58e3aded8896b2cbda479
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028786"
---
# <a name="get-user"></a><span data-ttu-id="7f9a1-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="7f9a1-103">Get user</span></span>

<span data-ttu-id="7f9a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f9a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f9a1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f9a1-106">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7f9a1-106">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f9a1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f9a1-107">Prerequisites</span></span>
<span data-ttu-id="7f9a1-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7f9a1-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9a1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7f9a1-110">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="7f9a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9a1-111">Permission type</span></span>|<span data-ttu-id="7f9a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f9a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f9a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f9a1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7f9a1-114">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="7f9a1-114">_varies by context_</span></span>|
| <span data-ttu-id="7f9a1-115">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="7f9a1-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="7f9a1-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9a1-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7f9a1-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="7f9a1-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7f9a1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9a1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7f9a1-119">&nbsp;Входящая миграция &nbsp;</span><span class="sxs-lookup"><span data-stu-id="7f9a1-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="7f9a1-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9a1-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7f9a1-121">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="7f9a1-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7f9a1-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9a1-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="7f9a1-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f9a1-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f9a1-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-124">Not supported.</span></span>|
|<span data-ttu-id="7f9a1-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f9a1-125">Application</span></span>|<span data-ttu-id="7f9a1-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f9a1-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f9a1-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f9a1-128">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7f9a1-128">Optional query parameters</span></span>
<span data-ttu-id="7f9a1-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f9a1-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f9a1-130">Request headers</span></span>
|<span data-ttu-id="7f9a1-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f9a1-131">Header</span></span>|<span data-ttu-id="7f9a1-132">Значение</span><span class="sxs-lookup"><span data-stu-id="7f9a1-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f9a1-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f9a1-133">Authorization</span></span>|<span data-ttu-id="7f9a1-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f9a1-135">Accept</span><span class="sxs-lookup"><span data-stu-id="7f9a1-135">Accept</span></span>|<span data-ttu-id="7f9a1-136">application/json</span><span class="sxs-lookup"><span data-stu-id="7f9a1-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f9a1-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f9a1-137">Request body</span></span>
<span data-ttu-id="7f9a1-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f9a1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9a1-139">Response</span></span>
<span data-ttu-id="7f9a1-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f9a1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7f9a1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f9a1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9a1-142">Request</span></span>
<span data-ttu-id="7f9a1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="7f9a1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9a1-144">Response</span></span>
<span data-ttu-id="7f9a1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f9a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









