---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4bca90bc1e42b6dde596d22d2bd1e42dcc5910db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979469"
---
# <a name="get-user"></a><span data-ttu-id="b948c-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="b948c-103">Get user</span></span>

> <span data-ttu-id="b948c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b948c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b948c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b948c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b948c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b948c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b948c-107">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="b948c-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b948c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b948c-108">Prerequisites</span></span>

<span data-ttu-id="b948c-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b948c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b948c-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b948c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b948c-111">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="b948c-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="b948c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b948c-112">Permission type</span></span>|<span data-ttu-id="b948c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b948c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b948c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b948c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b948c-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b948c-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b948c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b948c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b948c-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="b948c-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="b948c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b948c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b948c-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="b948c-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b948c-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b948c-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b948c-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b948c-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b948c-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b948c-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="b948c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b948c-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b948c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b948c-124">Not supported.</span></span>|
|<span data-ttu-id="b948c-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b948c-125">Application</span></span>|<span data-ttu-id="b948c-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b948c-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b948c-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b948c-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b948c-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b948c-128">Optional query parameters</span></span>

<span data-ttu-id="b948c-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b948c-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b948c-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b948c-130">Request headers</span></span>

|<span data-ttu-id="b948c-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b948c-131">Header</span></span>|<span data-ttu-id="b948c-132">Значение</span><span class="sxs-lookup"><span data-stu-id="b948c-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b948c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="b948c-133">Authorization</span></span>|<span data-ttu-id="b948c-134">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b948c-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b948c-135">Accept</span><span class="sxs-lookup"><span data-stu-id="b948c-135">Accept</span></span>|<span data-ttu-id="b948c-136">application/json</span><span class="sxs-lookup"><span data-stu-id="b948c-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b948c-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b948c-137">Request body</span></span>

<span data-ttu-id="b948c-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b948c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b948c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b948c-139">Response</span></span>

<span data-ttu-id="b948c-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b948c-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b948c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b948c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b948c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b948c-142">Request</span></span>

<span data-ttu-id="b948c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b948c-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="b948c-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b948c-144">Response</span></span>

<span data-ttu-id="b948c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b948c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



