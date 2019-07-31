---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67fabcf6f369db297d104f2273969b4682475084
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979675"
---
# <a name="get-user"></a><span data-ttu-id="c7afa-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="c7afa-103">Get user</span></span>

> <span data-ttu-id="c7afa-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7afa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7afa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7afa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7afa-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7afa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7afa-107">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c7afa-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7afa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7afa-108">Prerequisites</span></span>

<span data-ttu-id="c7afa-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="c7afa-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c7afa-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7afa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c7afa-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c7afa-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="c7afa-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7afa-112">Permission type</span></span>|<span data-ttu-id="c7afa-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7afa-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7afa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7afa-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c7afa-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c7afa-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c7afa-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7afa-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c7afa-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c7afa-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c7afa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7afa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c7afa-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c7afa-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c7afa-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7afa-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c7afa-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c7afa-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c7afa-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7afa-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="c7afa-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7afa-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7afa-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7afa-124">Not supported.</span></span>|
|<span data-ttu-id="c7afa-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7afa-125">Application</span></span>|<span data-ttu-id="c7afa-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7afa-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7afa-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7afa-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7afa-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7afa-128">Optional query parameters</span></span>

<span data-ttu-id="c7afa-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7afa-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7afa-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7afa-130">Request headers</span></span>

|<span data-ttu-id="c7afa-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7afa-131">Header</span></span>|<span data-ttu-id="c7afa-132">Значение</span><span class="sxs-lookup"><span data-stu-id="c7afa-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7afa-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7afa-133">Authorization</span></span>|<span data-ttu-id="c7afa-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7afa-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7afa-135">Accept</span><span class="sxs-lookup"><span data-stu-id="c7afa-135">Accept</span></span>|<span data-ttu-id="c7afa-136">application/json</span><span class="sxs-lookup"><span data-stu-id="c7afa-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7afa-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7afa-137">Request body</span></span>

<span data-ttu-id="c7afa-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7afa-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7afa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7afa-139">Response</span></span>

<span data-ttu-id="c7afa-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7afa-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7afa-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c7afa-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7afa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7afa-142">Request</span></span>

<span data-ttu-id="c7afa-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7afa-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c7afa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7afa-144">Response</span></span>

<span data-ttu-id="c7afa-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7afa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



