---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
ms.openlocfilehash: 619f35e5b7e8ffd75a8bcd2db32122dd69a9ac2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026995"
---
# <a name="get-user"></a><span data-ttu-id="29ab9-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="29ab9-103">Get user</span></span>

> <span data-ttu-id="29ab9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29ab9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29ab9-105">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="29ab9-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29ab9-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="29ab9-106">Prerequisites</span></span>
<span data-ttu-id="29ab9-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="29ab9-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="29ab9-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29ab9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="29ab9-109">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="29ab9-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="29ab9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29ab9-110">Permission type</span></span>|<span data-ttu-id="29ab9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29ab9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29ab9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29ab9-112">Delegated (work or school account)</span></span>| <span data-ttu-id="29ab9-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="29ab9-113">_varies by context_</span></span>|
| <span data-ttu-id="29ab9-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="29ab9-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="29ab9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ab9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="29ab9-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="29ab9-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="29ab9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ab9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="29ab9-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="29ab9-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="29ab9-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ab9-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="29ab9-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="29ab9-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="29ab9-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29ab9-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="29ab9-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29ab9-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29ab9-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ab9-123">Not supported.</span></span>|
|<span data-ttu-id="29ab9-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29ab9-124">Application</span></span>|<span data-ttu-id="29ab9-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ab9-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29ab9-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29ab9-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29ab9-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29ab9-127">Optional query parameters</span></span>
<span data-ttu-id="29ab9-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="29ab9-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29ab9-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29ab9-129">Request headers</span></span>
|<span data-ttu-id="29ab9-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29ab9-130">Header</span></span>|<span data-ttu-id="29ab9-131">Значение</span><span class="sxs-lookup"><span data-stu-id="29ab9-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29ab9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="29ab9-132">Authorization</span></span>|<span data-ttu-id="29ab9-133">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="29ab9-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29ab9-134">Accept</span><span class="sxs-lookup"><span data-stu-id="29ab9-134">Accept</span></span>|<span data-ttu-id="29ab9-135">application/json</span><span class="sxs-lookup"><span data-stu-id="29ab9-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ab9-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29ab9-136">Request body</span></span>
<span data-ttu-id="29ab9-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29ab9-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29ab9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="29ab9-138">Response</span></span>
<span data-ttu-id="29ab9-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29ab9-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ab9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="29ab9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="29ab9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="29ab9-141">Request</span></span>
<span data-ttu-id="29ab9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29ab9-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="29ab9-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="29ab9-143">Response</span></span>
<span data-ttu-id="29ab9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="29ab9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



