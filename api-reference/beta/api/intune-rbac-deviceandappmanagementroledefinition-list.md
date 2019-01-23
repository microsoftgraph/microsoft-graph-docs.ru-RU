---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ed74b1fb338a2ffd419e6245ae86f55698d844f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395218"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="e3e4d-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3e4d-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="e3e4d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3e4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3e4d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e4d-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e3e4d-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3e4d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3e4d-108">Prerequisites</span></span>
<span data-ttu-id="e3e4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3e4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3e4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3e4d-111">Permission type</span></span>|<span data-ttu-id="e3e4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3e4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3e4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e4d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3e4d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e3e4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3e4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-116">Not supported.</span></span>|
|<span data-ttu-id="e3e4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3e4d-117">Application</span></span>|<span data-ttu-id="e3e4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3e4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e3e4d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3e4d-120">Request headers</span></span>
|<span data-ttu-id="e3e4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3e4d-121">Header</span></span>|<span data-ttu-id="e3e4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3e4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e4d-123">Authorization</span></span>|<span data-ttu-id="e3e4d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3e4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3e4d-125">Accept</span></span>|<span data-ttu-id="e3e4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3e4d-127">Request body</span></span>
<span data-ttu-id="e3e4d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3e4d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e4d-129">Response</span></span>
<span data-ttu-id="e3e4d-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e4d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e3e4d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3e4d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3e4d-132">Request</span></span>
<span data-ttu-id="e3e4d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="e3e4d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e4d-134">Response</span></span>
<span data-ttu-id="e3e4d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3e4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




