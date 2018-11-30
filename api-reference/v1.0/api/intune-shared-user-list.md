---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
ms.openlocfilehash: 06044d50bf21e52f61a66a7e54b11c69c9e5f700
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027490"
---
# <a name="list-users"></a><span data-ttu-id="2bcf5-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="2bcf5-103">List users</span></span>

> <span data-ttu-id="2bcf5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bcf5-105">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="2bcf5-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bcf5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2bcf5-106">Prerequisites</span></span>
<span data-ttu-id="2bcf5-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2bcf5-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bcf5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="2bcf5-109">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="2bcf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bcf5-110">Permission type</span></span>|<span data-ttu-id="2bcf5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bcf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bcf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bcf5-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2bcf5-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="2bcf5-113">_varies by context_</span></span>|
| <span data-ttu-id="2bcf5-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="2bcf5-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="2bcf5-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bcf5-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="2bcf5-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="2bcf5-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="2bcf5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bcf5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="2bcf5-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="2bcf5-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="2bcf5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bcf5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="2bcf5-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="2bcf5-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="2bcf5-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bcf5-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="2bcf5-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bcf5-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bcf5-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-123">Not supported.</span></span>|
|<span data-ttu-id="2bcf5-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bcf5-124">Application</span></span>|<span data-ttu-id="2bcf5-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bcf5-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bcf5-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="2bcf5-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bcf5-127">Request headers</span></span>
|<span data-ttu-id="2bcf5-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bcf5-128">Header</span></span>|<span data-ttu-id="2bcf5-129">Значение</span><span class="sxs-lookup"><span data-stu-id="2bcf5-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bcf5-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bcf5-130">Authorization</span></span>|<span data-ttu-id="2bcf5-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2bcf5-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bcf5-132">Accept</span><span class="sxs-lookup"><span data-stu-id="2bcf5-132">Accept</span></span>|<span data-ttu-id="2bcf5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2bcf5-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bcf5-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bcf5-134">Request body</span></span>
<span data-ttu-id="2bcf5-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bcf5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bcf5-136">Response</span></span>
<span data-ttu-id="2bcf5-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bcf5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2bcf5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bcf5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bcf5-139">Request</span></span>
<span data-ttu-id="2bcf5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bcf5-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="2bcf5-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bcf5-141">Response</span></span>
<span data-ttu-id="2bcf5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2bcf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



