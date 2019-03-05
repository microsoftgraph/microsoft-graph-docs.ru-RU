---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a97f8e774d7f3ccb855ff8f9c923bbc8109581f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255124"
---
# <a name="get-auditevent"></a><span data-ttu-id="6338f-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="6338f-103">Get auditEvent</span></span>

> <span data-ttu-id="6338f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6338f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6338f-105">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="6338f-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6338f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6338f-106">Prerequisites</span></span>
<span data-ttu-id="6338f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6338f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6338f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6338f-109">Permission type</span></span>|<span data-ttu-id="6338f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6338f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6338f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6338f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6338f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6338f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6338f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6338f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6338f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6338f-114">Not supported.</span></span>|
|<span data-ttu-id="6338f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6338f-115">Application</span></span>|<span data-ttu-id="6338f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6338f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6338f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6338f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6338f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6338f-118">Optional query parameters</span></span>
<span data-ttu-id="6338f-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6338f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6338f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6338f-120">Request headers</span></span>
|<span data-ttu-id="6338f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6338f-121">Header</span></span>|<span data-ttu-id="6338f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6338f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6338f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6338f-123">Authorization</span></span>|<span data-ttu-id="6338f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6338f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6338f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6338f-125">Accept</span></span>|<span data-ttu-id="6338f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6338f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6338f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6338f-127">Request body</span></span>
<span data-ttu-id="6338f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6338f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6338f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6338f-129">Response</span></span>
<span data-ttu-id="6338f-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6338f-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6338f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6338f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6338f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6338f-132">Request</span></span>
<span data-ttu-id="6338f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6338f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="6338f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6338f-134">Response</span></span>
<span data-ttu-id="6338f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6338f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



