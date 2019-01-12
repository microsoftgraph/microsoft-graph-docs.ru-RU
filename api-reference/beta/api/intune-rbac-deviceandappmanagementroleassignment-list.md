---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d6d583c440b73ef1fac3d84d130183116b14a21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991055"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="7fe95-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7fe95-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="7fe95-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7fe95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fe95-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fe95-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7fe95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fe95-107">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7fe95-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fe95-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7fe95-108">Prerequisites</span></span>
<span data-ttu-id="7fe95-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe95-111">Permission type</span></span>|<span data-ttu-id="7fe95-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fe95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fe95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe95-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fe95-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7fe95-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fe95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe95-116">Not supported.</span></span>|
|<span data-ttu-id="7fe95-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fe95-117">Application</span></span>|<span data-ttu-id="7fe95-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe95-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fe95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7fe95-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fe95-120">Request headers</span></span>
|<span data-ttu-id="7fe95-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fe95-121">Header</span></span>|<span data-ttu-id="7fe95-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7fe95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fe95-123">Authorization</span></span>|<span data-ttu-id="7fe95-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7fe95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe95-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fe95-125">Accept</span></span>|<span data-ttu-id="7fe95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe95-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fe95-127">Request body</span></span>
<span data-ttu-id="7fe95-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fe95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe95-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe95-129">Response</span></span>
<span data-ttu-id="7fe95-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe95-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe95-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7fe95-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fe95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fe95-132">Request</span></span>
<span data-ttu-id="7fe95-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe95-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="7fe95-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fe95-134">Response</span></span>
<span data-ttu-id="7fe95-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7fe95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "members": [
        "Members value"
      ]
    }
  ]
}
```





