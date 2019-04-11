---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac6fddfbb25cdaa0be4b2e2dc15481f8945f2069
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775368"
---
# <a name="get-auditevent"></a><span data-ttu-id="c9937-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="c9937-103">Get auditEvent</span></span>

> <span data-ttu-id="c9937-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9937-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9937-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9937-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9937-106">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="c9937-106">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9937-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c9937-107">Prerequisites</span></span>
<span data-ttu-id="c9937-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9937-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9937-110">Permission type</span></span>|<span data-ttu-id="c9937-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9937-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9937-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9937-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9937-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9937-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c9937-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9937-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9937-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9937-115">Not supported.</span></span>|
|<span data-ttu-id="c9937-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9937-116">Application</span></span>|<span data-ttu-id="c9937-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9937-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9937-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9937-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9937-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9937-119">Optional query parameters</span></span>
<span data-ttu-id="c9937-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9937-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9937-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9937-121">Request headers</span></span>
|<span data-ttu-id="c9937-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9937-122">Header</span></span>|<span data-ttu-id="c9937-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c9937-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9937-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9937-124">Authorization</span></span>|<span data-ttu-id="c9937-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9937-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9937-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c9937-126">Accept</span></span>|<span data-ttu-id="c9937-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c9937-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9937-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9937-128">Request body</span></span>
<span data-ttu-id="c9937-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9937-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9937-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9937-130">Response</span></span>
<span data-ttu-id="c9937-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9937-131">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9937-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c9937-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9937-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9937-133">Request</span></span>
<span data-ttu-id="c9937-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9937-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="c9937-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9937-135">Response</span></span>
<span data-ttu-id="c9937-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9937-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





