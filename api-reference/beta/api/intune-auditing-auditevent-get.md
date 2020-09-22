---
title: Get auditEvent
description: Чтение свойств и связей объекта auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: deab078a47210eaca9a785caff6618827706f1fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975936"
---
# <a name="get-auditevent"></a><span data-ttu-id="2a95b-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="2a95b-103">Get auditEvent</span></span>

<span data-ttu-id="2a95b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a95b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a95b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a95b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a95b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a95b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a95b-107">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="2a95b-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a95b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2a95b-108">Prerequisites</span></span>
<span data-ttu-id="2a95b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a95b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a95b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a95b-111">Permission type</span></span>|<span data-ttu-id="2a95b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a95b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a95b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a95b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a95b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a95b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2a95b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a95b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a95b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a95b-116">Not supported.</span></span>|
|<span data-ttu-id="2a95b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a95b-117">Application</span></span>|<span data-ttu-id="2a95b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a95b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a95b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a95b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a95b-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2a95b-120">Optional query parameters</span></span>
<span data-ttu-id="2a95b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a95b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a95b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a95b-122">Request headers</span></span>
|<span data-ttu-id="2a95b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a95b-123">Header</span></span>|<span data-ttu-id="2a95b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2a95b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a95b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a95b-125">Authorization</span></span>|<span data-ttu-id="2a95b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a95b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a95b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2a95b-127">Accept</span></span>|<span data-ttu-id="2a95b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2a95b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a95b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a95b-129">Request body</span></span>
<span data-ttu-id="2a95b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a95b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a95b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a95b-131">Response</span></span>
<span data-ttu-id="2a95b-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune-auditing-auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a95b-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a95b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2a95b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a95b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a95b-134">Request</span></span>
<span data-ttu-id="2a95b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a95b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="2a95b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a95b-136">Response</span></span>
<span data-ttu-id="2a95b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a95b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1863

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
      "userId": "User Id value",
      "userRoleScopeTags": [
        {
          "@odata.type": "microsoft.graph.roleScopeTagInfo",
          "displayName": "Display Name value",
          "roleScopeTagId": "Role Scope Tag Id value"
        }
      ],
      "remoteTenantId": "Remote Tenant Id value",
      "remoteUserId": "Remote User Id value"
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






