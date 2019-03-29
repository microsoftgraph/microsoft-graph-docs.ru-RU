---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e6643fa2beccf83384c454451094473e7c80ac8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970963"
---
# <a name="get-user"></a><span data-ttu-id="9cc7d-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="9cc7d-103">Get user</span></span>

> <span data-ttu-id="9cc7d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cc7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cc7d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cc7d-107">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7d-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cc7d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9cc7d-108">Prerequisites</span></span>

<span data-ttu-id="9cc7d-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9cc7d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc7d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9cc7d-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="9cc7d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cc7d-112">Permission type</span></span>|<span data-ttu-id="9cc7d-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cc7d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc7d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cc7d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9cc7d-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9cc7d-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc7d-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="9cc7d-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="9cc7d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc7d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="9cc7d-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9cc7d-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc7d-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="9cc7d-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="9cc7d-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc7d-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="9cc7d-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cc7d-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc7d-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-124">Not supported.</span></span>|
|<span data-ttu-id="9cc7d-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cc7d-125">Application</span></span>|<span data-ttu-id="9cc7d-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc7d-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cc7d-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cc7d-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9cc7d-128">Optional query parameters</span></span>

<span data-ttu-id="9cc7d-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cc7d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cc7d-130">Request headers</span></span>

|<span data-ttu-id="9cc7d-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cc7d-131">Header</span></span>|<span data-ttu-id="9cc7d-132">Значение</span><span class="sxs-lookup"><span data-stu-id="9cc7d-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc7d-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cc7d-133">Authorization</span></span>|<span data-ttu-id="9cc7d-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc7d-135">Accept</span><span class="sxs-lookup"><span data-stu-id="9cc7d-135">Accept</span></span>|<span data-ttu-id="9cc7d-136">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc7d-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc7d-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cc7d-137">Request body</span></span>

<span data-ttu-id="9cc7d-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cc7d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc7d-139">Response</span></span>

<span data-ttu-id="9cc7d-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc7d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9cc7d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cc7d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cc7d-142">Request</span></span>

<span data-ttu-id="9cc7d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="9cc7d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc7d-144">Response</span></span>

<span data-ttu-id="9cc7d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



