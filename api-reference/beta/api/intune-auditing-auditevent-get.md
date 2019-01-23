---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0d3e0450a80bc2b0932fda3143d14d46e30fb89
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421034"
---
# <a name="get-auditevent"></a><span data-ttu-id="1f702-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="1f702-103">Get auditEvent</span></span>

> <span data-ttu-id="1f702-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f702-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f702-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f702-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f702-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f702-107">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="1f702-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f702-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1f702-108">Prerequisites</span></span>
<span data-ttu-id="1f702-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f702-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f702-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f702-111">Permission type</span></span>|<span data-ttu-id="1f702-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f702-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f702-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f702-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f702-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f702-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1f702-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f702-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f702-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f702-116">Not supported.</span></span>|
|<span data-ttu-id="1f702-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f702-117">Application</span></span>|<span data-ttu-id="1f702-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f702-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f702-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f702-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f702-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f702-120">Optional query parameters</span></span>
<span data-ttu-id="1f702-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f702-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f702-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f702-122">Request headers</span></span>
|<span data-ttu-id="1f702-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f702-123">Header</span></span>|<span data-ttu-id="1f702-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1f702-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f702-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f702-125">Authorization</span></span>|<span data-ttu-id="1f702-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1f702-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f702-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1f702-127">Accept</span></span>|<span data-ttu-id="1f702-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f702-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f702-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f702-129">Request body</span></span>
<span data-ttu-id="1f702-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f702-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f702-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f702-131">Response</span></span>
<span data-ttu-id="1f702-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1f702-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f702-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f702-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f702-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f702-134">Request</span></span>
<span data-ttu-id="1f702-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f702-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="1f702-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f702-136">Response</span></span>
<span data-ttu-id="1f702-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1f702-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




