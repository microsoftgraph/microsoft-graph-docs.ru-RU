---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 16fe6273ec71c37f0ef6408e3671f42fadcc6123
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959715"
---
# <a name="list-users"></a><span data-ttu-id="01aa6-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="01aa6-103">List users</span></span>

> <span data-ttu-id="01aa6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01aa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01aa6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01aa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01aa6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01aa6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01aa6-107">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="01aa6-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01aa6-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="01aa6-108">Prerequisites</span></span>

<span data-ttu-id="01aa6-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="01aa6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="01aa6-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01aa6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="01aa6-111">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="01aa6-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="01aa6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01aa6-112">Permission type</span></span>|<span data-ttu-id="01aa6-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01aa6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01aa6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01aa6-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="01aa6-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="01aa6-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="01aa6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01aa6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="01aa6-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="01aa6-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="01aa6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="01aa6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="01aa6-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="01aa6-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="01aa6-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="01aa6-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="01aa6-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="01aa6-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="01aa6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01aa6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="01aa6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01aa6-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01aa6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01aa6-124">Not supported.</span></span>|
|<span data-ttu-id="01aa6-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01aa6-125">Application</span></span>|<span data-ttu-id="01aa6-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01aa6-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01aa6-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01aa6-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="01aa6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01aa6-128">Request headers</span></span>

|<span data-ttu-id="01aa6-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01aa6-129">Header</span></span>|<span data-ttu-id="01aa6-130">Значение</span><span class="sxs-lookup"><span data-stu-id="01aa6-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01aa6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="01aa6-131">Authorization</span></span>|<span data-ttu-id="01aa6-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01aa6-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01aa6-133">Accept</span><span class="sxs-lookup"><span data-stu-id="01aa6-133">Accept</span></span>|<span data-ttu-id="01aa6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="01aa6-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01aa6-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01aa6-135">Request body</span></span>

<span data-ttu-id="01aa6-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01aa6-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01aa6-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="01aa6-137">Response</span></span>

<span data-ttu-id="01aa6-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01aa6-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01aa6-139">Пример</span><span class="sxs-lookup"><span data-stu-id="01aa6-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="01aa6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="01aa6-140">Request</span></span>

<span data-ttu-id="01aa6-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01aa6-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="01aa6-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="01aa6-142">Response</span></span>

<span data-ttu-id="01aa6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01aa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



