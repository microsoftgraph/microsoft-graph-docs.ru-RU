---
title: Перечисление объектов auditEvent
description: Список свойств и связей объектов auditEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 344e6a1413d95ede901d2cd6d3390ad83281af47
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839797"
---
# <a name="list-auditevents"></a><span data-ttu-id="70b67-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="70b67-103">List auditEvents</span></span>

> <span data-ttu-id="70b67-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="70b67-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70b67-105">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="70b67-105">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70b67-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="70b67-106">Prerequisites</span></span>
<span data-ttu-id="70b67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70b67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70b67-109">Permission type</span></span>|<span data-ttu-id="70b67-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70b67-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70b67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70b67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70b67-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70b67-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70b67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70b67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70b67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70b67-114">Not supported.</span></span>|
|<span data-ttu-id="70b67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70b67-115">Application</span></span>|<span data-ttu-id="70b67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70b67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70b67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70b67-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="70b67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70b67-118">Request headers</span></span>
|<span data-ttu-id="70b67-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70b67-119">Header</span></span>|<span data-ttu-id="70b67-120">Значение</span><span class="sxs-lookup"><span data-stu-id="70b67-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70b67-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70b67-121">Authorization</span></span>|<span data-ttu-id="70b67-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="70b67-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70b67-123">Accept</span><span class="sxs-lookup"><span data-stu-id="70b67-123">Accept</span></span>|<span data-ttu-id="70b67-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70b67-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70b67-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70b67-125">Request body</span></span>
<span data-ttu-id="70b67-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70b67-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70b67-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="70b67-127">Response</span></span>
<span data-ttu-id="70b67-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70b67-128">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70b67-129">Пример</span><span class="sxs-lookup"><span data-stu-id="70b67-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="70b67-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="70b67-130">Request</span></span>
<span data-ttu-id="70b67-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70b67-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="70b67-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="70b67-132">Response</span></span>
<span data-ttu-id="70b67-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="70b67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
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
  ]
}
```



