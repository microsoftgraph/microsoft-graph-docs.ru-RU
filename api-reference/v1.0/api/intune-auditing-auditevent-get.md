---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b711362bd9aecf38c863157c97136776a868d33a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354863"
---
# <a name="get-auditevent"></a><span data-ttu-id="37435-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="37435-103">Get auditEvent</span></span>

> <span data-ttu-id="37435-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37435-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37435-105">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="37435-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37435-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="37435-106">Prerequisites</span></span>
<span data-ttu-id="37435-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37435-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37435-109">Permission type</span></span>|<span data-ttu-id="37435-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37435-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37435-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37435-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37435-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37435-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="37435-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37435-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37435-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37435-114">Not supported.</span></span>|
|<span data-ttu-id="37435-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37435-115">Application</span></span>|<span data-ttu-id="37435-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37435-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37435-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37435-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37435-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37435-118">Optional query parameters</span></span>
<span data-ttu-id="37435-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37435-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37435-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37435-120">Request headers</span></span>
|<span data-ttu-id="37435-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37435-121">Header</span></span>|<span data-ttu-id="37435-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37435-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37435-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37435-123">Authorization</span></span>|<span data-ttu-id="37435-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37435-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37435-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37435-125">Accept</span></span>|<span data-ttu-id="37435-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37435-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37435-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37435-127">Request body</span></span>
<span data-ttu-id="37435-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37435-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37435-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="37435-129">Response</span></span>
<span data-ttu-id="37435-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37435-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37435-131">Пример</span><span class="sxs-lookup"><span data-stu-id="37435-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37435-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37435-132">Request</span></span>
<span data-ttu-id="37435-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37435-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="37435-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37435-134">Response</span></span>
<span data-ttu-id="37435-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37435-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




