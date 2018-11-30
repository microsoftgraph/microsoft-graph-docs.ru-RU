---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
ms.openlocfilehash: c1d803714b3d6fc4c813878a39e9231806b2795a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082014"
---
# <a name="list-users"></a><span data-ttu-id="7ba86-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="7ba86-103">List users</span></span>

> <span data-ttu-id="7ba86-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ba86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ba86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ba86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7ba86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ba86-107">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7ba86-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ba86-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ba86-108">Prerequisites</span></span>

<span data-ttu-id="7ba86-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="7ba86-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7ba86-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba86-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7ba86-111">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="7ba86-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="7ba86-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ba86-112">Permission type</span></span>|<span data-ttu-id="7ba86-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ba86-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ba86-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ba86-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7ba86-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="7ba86-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7ba86-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba86-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7ba86-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7ba86-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7ba86-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba86-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7ba86-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="7ba86-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7ba86-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba86-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7ba86-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="7ba86-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7ba86-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba86-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="7ba86-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ba86-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ba86-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba86-124">Not supported.</span></span>|
|<span data-ttu-id="7ba86-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ba86-125">Application</span></span>|<span data-ttu-id="7ba86-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba86-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ba86-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ba86-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="7ba86-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ba86-128">Request headers</span></span>

|<span data-ttu-id="7ba86-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ba86-129">Header</span></span>|<span data-ttu-id="7ba86-130">Значение</span><span class="sxs-lookup"><span data-stu-id="7ba86-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ba86-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ba86-131">Authorization</span></span>|<span data-ttu-id="7ba86-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7ba86-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ba86-133">Accept</span><span class="sxs-lookup"><span data-stu-id="7ba86-133">Accept</span></span>|<span data-ttu-id="7ba86-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7ba86-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba86-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ba86-135">Request body</span></span>

<span data-ttu-id="7ba86-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ba86-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba86-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ba86-137">Response</span></span>

<span data-ttu-id="7ba86-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ba86-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba86-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7ba86-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ba86-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ba86-140">Request</span></span>

<span data-ttu-id="7ba86-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ba86-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="7ba86-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ba86-142">Response</span></span>

<span data-ttu-id="7ba86-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7ba86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



