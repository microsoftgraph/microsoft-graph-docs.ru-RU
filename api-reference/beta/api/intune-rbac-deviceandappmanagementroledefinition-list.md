---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 642dd110923ee0d8b5a241373a7fb44f590baa50
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43421305"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="5ae9d-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ae9d-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="5ae9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ae9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ae9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ae9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae9d-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ae9d-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ae9d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5ae9d-108">Prerequisites</span></span>
<span data-ttu-id="5ae9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae9d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ae9d-111">Permission type</span></span>|<span data-ttu-id="5ae9d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ae9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae9d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ae9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae9d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ae9d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5ae9d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ae9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-116">Not supported.</span></span>|
|<span data-ttu-id="5ae9d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ae9d-117">Application</span></span>|<span data-ttu-id="5ae9d-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ae9d-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ae9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5ae9d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ae9d-120">Request headers</span></span>
|<span data-ttu-id="5ae9d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ae9d-121">Header</span></span>|<span data-ttu-id="5ae9d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ae9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ae9d-123">Authorization</span></span>|<span data-ttu-id="5ae9d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ae9d-125">Accept</span></span>|<span data-ttu-id="5ae9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae9d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ae9d-127">Request body</span></span>
<span data-ttu-id="5ae9d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ae9d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ae9d-129">Response</span></span>
<span data-ttu-id="5ae9d-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae9d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5ae9d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ae9d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ae9d-132">Request</span></span>
<span data-ttu-id="5ae9d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="5ae9d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae9d-134">Response</span></span>
<span data-ttu-id="5ae9d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ae9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



