---
title: Перечисление объектов auditEvent
description: Список свойств и связей объектов auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e2c7440ea7c442554afcbba4697490dee166291
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966102"
---
# <a name="list-auditevents"></a><span data-ttu-id="361a0-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="361a0-103">List auditEvents</span></span>

<span data-ttu-id="361a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="361a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="361a0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="361a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="361a0-106">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="361a0-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="361a0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="361a0-107">Prerequisites</span></span>
<span data-ttu-id="361a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="361a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="361a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="361a0-110">Permission type</span></span>|<span data-ttu-id="361a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="361a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="361a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="361a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="361a0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="361a0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="361a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="361a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="361a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="361a0-115">Not supported.</span></span>|
|<span data-ttu-id="361a0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="361a0-116">Application</span></span>|<span data-ttu-id="361a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="361a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="361a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="361a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="361a0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="361a0-119">Request headers</span></span>
|<span data-ttu-id="361a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="361a0-120">Header</span></span>|<span data-ttu-id="361a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="361a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="361a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="361a0-122">Authorization</span></span>|<span data-ttu-id="361a0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="361a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="361a0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="361a0-124">Accept</span></span>|<span data-ttu-id="361a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="361a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="361a0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="361a0-126">Request body</span></span>
<span data-ttu-id="361a0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="361a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="361a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="361a0-128">Response</span></span>
<span data-ttu-id="361a0-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="361a0-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="361a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="361a0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="361a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="361a0-131">Request</span></span>
<span data-ttu-id="361a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="361a0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="361a0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="361a0-133">Response</span></span>
<span data-ttu-id="361a0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="361a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









