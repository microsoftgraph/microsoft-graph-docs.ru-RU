---
title: Перечисление объектов auditEvent
description: Список свойств и связей объектов auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10bde94668b7814d1ed110f5da8dab5a7daad3ef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131899"
---
# <a name="list-auditevents"></a><span data-ttu-id="c825c-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="c825c-103">List auditEvents</span></span>

<span data-ttu-id="c825c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c825c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c825c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c825c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c825c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c825c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c825c-107">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="c825c-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c825c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c825c-108">Prerequisites</span></span>
<span data-ttu-id="c825c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c825c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c825c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c825c-111">Permission type</span></span>|<span data-ttu-id="c825c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c825c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c825c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c825c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c825c-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c825c-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c825c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c825c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c825c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c825c-116">Not supported.</span></span>|
|<span data-ttu-id="c825c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c825c-117">Application</span></span>|<span data-ttu-id="c825c-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c825c-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c825c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c825c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="c825c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c825c-120">Request headers</span></span>
|<span data-ttu-id="c825c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c825c-121">Header</span></span>|<span data-ttu-id="c825c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c825c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c825c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c825c-123">Authorization</span></span>|<span data-ttu-id="c825c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c825c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c825c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c825c-125">Accept</span></span>|<span data-ttu-id="c825c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c825c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c825c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c825c-127">Request body</span></span>
<span data-ttu-id="c825c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c825c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c825c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c825c-129">Response</span></span>
<span data-ttu-id="c825c-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c825c-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c825c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c825c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c825c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c825c-132">Request</span></span>
<span data-ttu-id="c825c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c825c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="c825c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c825c-134">Response</span></span>
<span data-ttu-id="c825c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c825c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1975

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
  ]
}
```




