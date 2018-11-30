---
title: Перечисление объектов resourceOperation
description: Список свойств и связей объектов resourceOperation.
ms.openlocfilehash: 7110a16e2713e950d5018d4904272feddbd56dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079025"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="3f996-103">Перечисление объектов resourceOperation</span><span class="sxs-lookup"><span data-stu-id="3f996-103">List resourceOperations</span></span>

> <span data-ttu-id="3f996-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f996-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f996-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f996-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f996-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f996-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f996-107">Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3f996-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f996-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3f996-108">Prerequisites</span></span>
<span data-ttu-id="3f996-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f996-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f996-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f996-111">Permission type</span></span>|<span data-ttu-id="3f996-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f996-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f996-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f996-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f996-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f996-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3f996-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f996-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f996-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f996-116">Not supported.</span></span>|
|<span data-ttu-id="3f996-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f996-117">Application</span></span>|<span data-ttu-id="3f996-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f996-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f996-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f996-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="3f996-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f996-120">Request headers</span></span>
|<span data-ttu-id="3f996-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f996-121">Header</span></span>|<span data-ttu-id="3f996-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f996-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f996-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f996-123">Authorization</span></span>|<span data-ttu-id="3f996-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3f996-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f996-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f996-125">Accept</span></span>|<span data-ttu-id="3f996-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f996-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f996-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f996-127">Request body</span></span>
<span data-ttu-id="3f996-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f996-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f996-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f996-129">Response</span></span>
<span data-ttu-id="3f996-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3f996-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f996-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3f996-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f996-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f996-132">Request</span></span>
<span data-ttu-id="3f996-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f996-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="3f996-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f996-134">Response</span></span>
<span data-ttu-id="3f996-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3f996-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```





