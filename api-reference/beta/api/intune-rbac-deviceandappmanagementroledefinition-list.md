---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff3db2c2349c813bda3170f33645afc35f2230e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351471"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="84c1c-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="84c1c-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="84c1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84c1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84c1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84c1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84c1c-106">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="84c1c-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84c1c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="84c1c-107">Prerequisites</span></span>
<span data-ttu-id="84c1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84c1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84c1c-110">Permission type</span></span>|<span data-ttu-id="84c1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84c1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84c1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84c1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84c1c-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="84c1c-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="84c1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84c1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84c1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84c1c-115">Not supported.</span></span>|
|<span data-ttu-id="84c1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84c1c-116">Application</span></span>|<span data-ttu-id="84c1c-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="84c1c-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84c1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84c1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="84c1c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84c1c-119">Request headers</span></span>
|<span data-ttu-id="84c1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84c1c-120">Header</span></span>|<span data-ttu-id="84c1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="84c1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84c1c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84c1c-122">Authorization</span></span>|<span data-ttu-id="84c1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84c1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84c1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="84c1c-124">Accept</span></span>|<span data-ttu-id="84c1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84c1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84c1c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84c1c-126">Request body</span></span>
<span data-ttu-id="84c1c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84c1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84c1c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="84c1c-128">Response</span></span>
<span data-ttu-id="84c1c-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84c1c-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84c1c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="84c1c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84c1c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="84c1c-131">Request</span></span>
<span data-ttu-id="84c1c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84c1c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="84c1c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="84c1c-133">Response</span></span>
<span data-ttu-id="84c1c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84c1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

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
      "isBuiltIn": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






