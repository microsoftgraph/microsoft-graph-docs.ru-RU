---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7bb4547fa96cfd1492e3a4a1e7e0c73a42c3aad0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253143"
---
# <a name="get-user"></a><span data-ttu-id="0992e-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="0992e-103">Get user</span></span>

> <span data-ttu-id="0992e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0992e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0992e-105">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="0992e-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0992e-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0992e-106">Prerequisites</span></span>
<span data-ttu-id="0992e-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="0992e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0992e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0992e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="0992e-109">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="0992e-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="0992e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0992e-110">Permission type</span></span>|<span data-ttu-id="0992e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0992e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0992e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0992e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0992e-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="0992e-113">_varies by context_</span></span>|
| <span data-ttu-id="0992e-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="0992e-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="0992e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0992e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="0992e-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="0992e-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="0992e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0992e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="0992e-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="0992e-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0992e-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0992e-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0992e-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="0992e-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="0992e-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0992e-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="0992e-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0992e-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0992e-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0992e-123">Not supported.</span></span>|
|<span data-ttu-id="0992e-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0992e-124">Application</span></span>|<span data-ttu-id="0992e-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0992e-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0992e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0992e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0992e-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0992e-127">Optional query parameters</span></span>
<span data-ttu-id="0992e-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0992e-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0992e-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0992e-129">Request headers</span></span>
|<span data-ttu-id="0992e-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0992e-130">Header</span></span>|<span data-ttu-id="0992e-131">Значение</span><span class="sxs-lookup"><span data-stu-id="0992e-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0992e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0992e-132">Authorization</span></span>|<span data-ttu-id="0992e-133">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0992e-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0992e-134">Accept</span><span class="sxs-lookup"><span data-stu-id="0992e-134">Accept</span></span>|<span data-ttu-id="0992e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="0992e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0992e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0992e-136">Request body</span></span>
<span data-ttu-id="0992e-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0992e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0992e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0992e-138">Response</span></span>
<span data-ttu-id="0992e-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0992e-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0992e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0992e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0992e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0992e-141">Request</span></span>
<span data-ttu-id="0992e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0992e-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="0992e-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="0992e-143">Response</span></span>
<span data-ttu-id="0992e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0992e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



