---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0fe1ab86e78e4bff46a6c9105048519a20c894a1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141239"
---
# <a name="list-users"></a><span data-ttu-id="fa455-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="fa455-103">List users</span></span>

> <span data-ttu-id="fa455-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa455-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa455-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa455-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa455-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa455-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa455-107">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="fa455-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa455-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa455-108">Prerequisites</span></span>

<span data-ttu-id="fa455-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="fa455-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fa455-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa455-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="fa455-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="fa455-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="fa455-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa455-112">Permission type</span></span>|<span data-ttu-id="fa455-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa455-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa455-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa455-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fa455-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fa455-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fa455-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa455-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="fa455-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="fa455-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="fa455-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa455-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="fa455-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="fa455-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fa455-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa455-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="fa455-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="fa455-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fa455-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa455-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="fa455-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa455-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa455-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa455-124">Not supported.</span></span>|
|<span data-ttu-id="fa455-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa455-125">Application</span></span>|<span data-ttu-id="fa455-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa455-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa455-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa455-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="fa455-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa455-128">Request headers</span></span>

|<span data-ttu-id="fa455-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa455-129">Header</span></span>|<span data-ttu-id="fa455-130">Значение</span><span class="sxs-lookup"><span data-stu-id="fa455-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa455-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa455-131">Authorization</span></span>|<span data-ttu-id="fa455-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fa455-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa455-133">Accept</span><span class="sxs-lookup"><span data-stu-id="fa455-133">Accept</span></span>|<span data-ttu-id="fa455-134">application/json</span><span class="sxs-lookup"><span data-stu-id="fa455-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa455-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa455-135">Request body</span></span>

<span data-ttu-id="fa455-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa455-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa455-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa455-137">Response</span></span>

<span data-ttu-id="fa455-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa455-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa455-139">Пример</span><span class="sxs-lookup"><span data-stu-id="fa455-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa455-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa455-140">Request</span></span>

<span data-ttu-id="fa455-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa455-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="fa455-142">Отклик
</span><span class="sxs-lookup"><span data-stu-id="fa455-142">Response</span></span>

<span data-ttu-id="fa455-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fa455-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



