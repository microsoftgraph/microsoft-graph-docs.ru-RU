---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6ac6ccc3f1faccd6c158ae14f0a2696ec5e8684f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864836"
---
# <a name="get-auditevent"></a><span data-ttu-id="16f12-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="16f12-103">Get auditEvent</span></span>

> <span data-ttu-id="16f12-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16f12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16f12-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16f12-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16f12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16f12-107">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="16f12-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16f12-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="16f12-108">Prerequisites</span></span>
<span data-ttu-id="16f12-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16f12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16f12-111">Permission type</span></span>|<span data-ttu-id="16f12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16f12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16f12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16f12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16f12-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16f12-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16f12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16f12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16f12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f12-116">Not supported.</span></span>|
|<span data-ttu-id="16f12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16f12-117">Application</span></span>|<span data-ttu-id="16f12-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16f12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16f12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16f12-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16f12-120">Optional query parameters</span></span>
<span data-ttu-id="16f12-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16f12-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="16f12-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16f12-122">Request headers</span></span>
|<span data-ttu-id="16f12-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16f12-123">Header</span></span>|<span data-ttu-id="16f12-124">Значение</span><span class="sxs-lookup"><span data-stu-id="16f12-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16f12-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16f12-125">Authorization</span></span>|<span data-ttu-id="16f12-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16f12-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16f12-127">Accept</span><span class="sxs-lookup"><span data-stu-id="16f12-127">Accept</span></span>|<span data-ttu-id="16f12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16f12-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16f12-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16f12-129">Request body</span></span>
<span data-ttu-id="16f12-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16f12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16f12-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="16f12-131">Response</span></span>
<span data-ttu-id="16f12-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16f12-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="16f12-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="16f12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="16f12-134">Request</span></span>
<span data-ttu-id="16f12-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16f12-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="16f12-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="16f12-136">Response</span></span>
<span data-ttu-id="16f12-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16f12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value"
    },
    "activity": "Activity value",
    "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "displayName": "Display Name value",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "displayName": "Display Name value",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "type": "Type value",
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```





