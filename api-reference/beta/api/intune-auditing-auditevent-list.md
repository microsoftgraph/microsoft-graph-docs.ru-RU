---
title: Перечисление объектов auditEvent
description: Список свойств и связей объектов auditEvent.
ms.openlocfilehash: 8b684ca2c70d7875c218d38d32f359313fa02ee3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080068"
---
# <a name="list-auditevents"></a><span data-ttu-id="b79de-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="b79de-103">List auditEvents</span></span>

> <span data-ttu-id="b79de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b79de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b79de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b79de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b79de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b79de-107">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="b79de-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b79de-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b79de-108">Prerequisites</span></span>
<span data-ttu-id="b79de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b79de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b79de-111">Permission type</span></span>|<span data-ttu-id="b79de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b79de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b79de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b79de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b79de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b79de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b79de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b79de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79de-116">Not supported.</span></span>|
|<span data-ttu-id="b79de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b79de-117">Application</span></span>|<span data-ttu-id="b79de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b79de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b79de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b79de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="b79de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b79de-120">Request headers</span></span>
|<span data-ttu-id="b79de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b79de-121">Header</span></span>|<span data-ttu-id="b79de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b79de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b79de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79de-123">Authorization</span></span>|<span data-ttu-id="b79de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b79de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b79de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b79de-125">Accept</span></span>|<span data-ttu-id="b79de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b79de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b79de-127">Request body</span></span>
<span data-ttu-id="b79de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b79de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b79de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b79de-129">Response</span></span>
<span data-ttu-id="b79de-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b79de-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b79de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b79de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b79de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b79de-132">Request</span></span>
<span data-ttu-id="b79de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b79de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="b79de-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b79de-134">Response</span></span>
<span data-ttu-id="b79de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b79de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





