---
title: Список объектов roleAssignment
description: Список свойств и связей объектов roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 534fdd1e971dc46033be4d07679969f2d1a4c221
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868098"
---
# <a name="list-roleassignments"></a><span data-ttu-id="10f52-103">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="10f52-103">List roleAssignments</span></span>

> <span data-ttu-id="10f52-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10f52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10f52-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10f52-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10f52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10f52-107">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="10f52-107">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10f52-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10f52-108">Prerequisites</span></span>
<span data-ttu-id="10f52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10f52-111">Permission type</span></span>|<span data-ttu-id="10f52-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10f52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f52-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10f52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10f52-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="10f52-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="10f52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10f52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f52-116">Not supported.</span></span>|
|<span data-ttu-id="10f52-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10f52-117">Application</span></span>|<span data-ttu-id="10f52-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10f52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="10f52-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10f52-120">Request headers</span></span>
|<span data-ttu-id="10f52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10f52-121">Header</span></span>|<span data-ttu-id="10f52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10f52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f52-123">Authorization</span></span>|<span data-ttu-id="10f52-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="10f52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10f52-125">Accept</span></span>|<span data-ttu-id="10f52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10f52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f52-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10f52-127">Request body</span></span>
<span data-ttu-id="10f52-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10f52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10f52-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="10f52-129">Response</span></span>
<span data-ttu-id="10f52-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10f52-130">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f52-131">Пример</span><span class="sxs-lookup"><span data-stu-id="10f52-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="10f52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="10f52-132">Request</span></span>
<span data-ttu-id="10f52-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10f52-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="10f52-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="10f52-134">Response</span></span>
<span data-ttu-id="10f52-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10f52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```





