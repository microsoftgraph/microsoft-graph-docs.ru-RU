---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b3981047311673be8c640a35dbc862416427fa31
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252513"
---
# <a name="list-users"></a><span data-ttu-id="3ff1d-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="3ff1d-103">List users</span></span>

> <span data-ttu-id="3ff1d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff1d-105">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3ff1d-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ff1d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3ff1d-106">Prerequisites</span></span>
<span data-ttu-id="3ff1d-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3ff1d-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff1d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="3ff1d-109">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="3ff1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff1d-110">Permission type</span></span>|<span data-ttu-id="3ff1d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ff1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ff1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ff1d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3ff1d-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="3ff1d-113">_varies by context_</span></span>|
| <span data-ttu-id="3ff1d-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="3ff1d-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="3ff1d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ff1d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="3ff1d-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="3ff1d-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="3ff1d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ff1d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="3ff1d-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="3ff1d-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="3ff1d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ff1d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3ff1d-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3ff1d-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3ff1d-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ff1d-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="3ff1d-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ff1d-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ff1d-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-123">Not supported.</span></span>|
|<span data-ttu-id="3ff1d-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ff1d-124">Application</span></span>|<span data-ttu-id="3ff1d-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ff1d-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ff1d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="3ff1d-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ff1d-127">Request headers</span></span>
|<span data-ttu-id="3ff1d-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ff1d-128">Header</span></span>|<span data-ttu-id="3ff1d-129">Значение</span><span class="sxs-lookup"><span data-stu-id="3ff1d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ff1d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ff1d-130">Authorization</span></span>|<span data-ttu-id="3ff1d-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3ff1d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ff1d-132">Accept</span><span class="sxs-lookup"><span data-stu-id="3ff1d-132">Accept</span></span>|<span data-ttu-id="3ff1d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff1d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ff1d-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ff1d-134">Request body</span></span>
<span data-ttu-id="3ff1d-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ff1d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ff1d-136">Response</span></span>
<span data-ttu-id="3ff1d-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ff1d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3ff1d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ff1d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ff1d-139">Request</span></span>
<span data-ttu-id="3ff1d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="3ff1d-141">Отклик
</span><span class="sxs-lookup"><span data-stu-id="3ff1d-141">Response</span></span>
<span data-ttu-id="3ff1d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3ff1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



