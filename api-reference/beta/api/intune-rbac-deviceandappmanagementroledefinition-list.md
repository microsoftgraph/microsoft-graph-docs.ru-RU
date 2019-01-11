---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ca7df9ecc957895794a28298fa7d8b9ed08c04e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885689"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="fff91-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="fff91-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="fff91-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fff91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fff91-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fff91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fff91-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fff91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fff91-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fff91-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fff91-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fff91-108">Prerequisites</span></span>
<span data-ttu-id="fff91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fff91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fff91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fff91-111">Permission type</span></span>|<span data-ttu-id="fff91-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fff91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fff91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fff91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fff91-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff91-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fff91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fff91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fff91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fff91-116">Not supported.</span></span>|
|<span data-ttu-id="fff91-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fff91-117">Application</span></span>|<span data-ttu-id="fff91-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fff91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fff91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fff91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="fff91-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fff91-120">Request headers</span></span>
|<span data-ttu-id="fff91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fff91-121">Header</span></span>|<span data-ttu-id="fff91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fff91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fff91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fff91-123">Authorization</span></span>|<span data-ttu-id="fff91-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fff91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fff91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fff91-125">Accept</span></span>|<span data-ttu-id="fff91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fff91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fff91-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fff91-127">Request body</span></span>
<span data-ttu-id="fff91-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fff91-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fff91-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fff91-129">Response</span></span>
<span data-ttu-id="fff91-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fff91-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fff91-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fff91-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fff91-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fff91-132">Request</span></span>
<span data-ttu-id="fff91-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fff91-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="fff91-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fff91-134">Response</span></span>
<span data-ttu-id="fff91-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fff91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1425

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "permissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "actions": [
            "Actions value"
          ],
          "resourceActions": [
            {
              "@odata.type": "microsoft.graph.resourceAction",
              "allowedResourceActions": [
                "Allowed Resource Actions value"
              ],
              "notAllowedResourceActions": [
                "Not Allowed Resource Actions value"
              ]
            }
          ]
        }
      ],
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "actions": [
            "Actions value"
          ],
          "resourceActions": [
            {
              "@odata.type": "microsoft.graph.resourceAction",
              "allowedResourceActions": [
                "Allowed Resource Actions value"
              ],
              "notAllowedResourceActions": [
                "Not Allowed Resource Actions value"
              ]
            }
          ]
        }
      ],
      "isBuiltInRoleDefinition": true,
      "isBuiltIn": true
    }
  ]
}
```





