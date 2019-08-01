---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50b5555943d5adede6d5c3d23fd3c8384cd29d9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023393"
---
# <a name="get-user"></a><span data-ttu-id="ec189-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="ec189-103">Get user</span></span>

> <span data-ttu-id="ec189-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec189-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec189-105">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="ec189-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec189-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec189-106">Prerequisites</span></span>
<span data-ttu-id="ec189-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec189-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ec189-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec189-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ec189-109">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="ec189-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="ec189-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec189-110">Permission type</span></span>|<span data-ttu-id="ec189-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec189-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec189-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec189-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ec189-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="ec189-113">_varies by context_</span></span>|
| <span data-ttu-id="ec189-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="ec189-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="ec189-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec189-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ec189-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="ec189-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="ec189-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec189-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ec189-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="ec189-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="ec189-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec189-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ec189-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="ec189-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="ec189-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec189-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="ec189-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec189-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec189-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec189-123">Not supported.</span></span>|
|<span data-ttu-id="ec189-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec189-124">Application</span></span>|<span data-ttu-id="ec189-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec189-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec189-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec189-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec189-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec189-127">Optional query parameters</span></span>
<span data-ttu-id="ec189-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec189-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ec189-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec189-129">Request headers</span></span>
|<span data-ttu-id="ec189-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec189-130">Header</span></span>|<span data-ttu-id="ec189-131">Значение</span><span class="sxs-lookup"><span data-stu-id="ec189-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec189-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec189-132">Authorization</span></span>|<span data-ttu-id="ec189-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec189-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec189-134">Accept</span><span class="sxs-lookup"><span data-stu-id="ec189-134">Accept</span></span>|<span data-ttu-id="ec189-135">application/json</span><span class="sxs-lookup"><span data-stu-id="ec189-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec189-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec189-136">Request body</span></span>
<span data-ttu-id="ec189-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec189-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec189-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec189-138">Response</span></span>
<span data-ttu-id="ec189-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec189-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec189-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ec189-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec189-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec189-141">Request</span></span>
<span data-ttu-id="ec189-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec189-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="ec189-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec189-143">Response</span></span>
<span data-ttu-id="ec189-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec189-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



