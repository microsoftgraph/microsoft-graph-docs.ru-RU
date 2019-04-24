---
title: Перечисление объектов auditEvent
description: Список свойств и связей объектов auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e52eaee297b587bba1d6d41afa21f11005dc835f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32484260"
---
# <a name="list-auditevents"></a><span data-ttu-id="a30fc-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="a30fc-103">List auditEvents</span></span>

> <span data-ttu-id="a30fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a30fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a30fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a30fc-106">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="a30fc-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a30fc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a30fc-107">Prerequisites</span></span>
<span data-ttu-id="a30fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a30fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a30fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a30fc-110">Permission type</span></span>|<span data-ttu-id="a30fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a30fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a30fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a30fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a30fc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a30fc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a30fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a30fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a30fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30fc-115">Not supported.</span></span>|
|<span data-ttu-id="a30fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a30fc-116">Application</span></span>|<span data-ttu-id="a30fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a30fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a30fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="a30fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a30fc-119">Request headers</span></span>
|<span data-ttu-id="a30fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a30fc-120">Header</span></span>|<span data-ttu-id="a30fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a30fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a30fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a30fc-122">Authorization</span></span>|<span data-ttu-id="a30fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a30fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a30fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a30fc-124">Accept</span></span>|<span data-ttu-id="a30fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a30fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a30fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a30fc-126">Request body</span></span>
<span data-ttu-id="a30fc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a30fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a30fc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a30fc-128">Response</span></span>
<span data-ttu-id="a30fc-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [auditEvent](../resources/intune-auditing-auditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a30fc-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a30fc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a30fc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a30fc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a30fc-131">Request</span></span>
<span data-ttu-id="a30fc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a30fc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="a30fc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a30fc-133">Response</span></span>
<span data-ttu-id="a30fc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a30fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





