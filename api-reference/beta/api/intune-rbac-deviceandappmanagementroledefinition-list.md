---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73f4cba0578f8510ca7f034ea415016dee49023e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148530"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="8c5b1-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8c5b1-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="8c5b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c5b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c5b1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c5b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c5b1-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8c5b1-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c5b1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c5b1-108">Prerequisites</span></span>
<span data-ttu-id="8c5b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c5b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c5b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c5b1-111">Permission type</span></span>|<span data-ttu-id="8c5b1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c5b1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c5b1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c5b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c5b1-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c5b1-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8c5b1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c5b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c5b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-116">Not supported.</span></span>|
|<span data-ttu-id="8c5b1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c5b1-117">Application</span></span>|<span data-ttu-id="8c5b1-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c5b1-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c5b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c5b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8c5b1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c5b1-120">Request headers</span></span>
|<span data-ttu-id="8c5b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c5b1-121">Header</span></span>|<span data-ttu-id="8c5b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c5b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c5b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c5b1-123">Authorization</span></span>|<span data-ttu-id="8c5b1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c5b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c5b1-125">Accept</span></span>|<span data-ttu-id="8c5b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c5b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c5b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c5b1-127">Request body</span></span>
<span data-ttu-id="8c5b1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c5b1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c5b1-129">Response</span></span>
<span data-ttu-id="8c5b1-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c5b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8c5b1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c5b1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c5b1-132">Request</span></span>
<span data-ttu-id="8c5b1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="8c5b1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c5b1-134">Response</span></span>
<span data-ttu-id="8c5b1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c5b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




