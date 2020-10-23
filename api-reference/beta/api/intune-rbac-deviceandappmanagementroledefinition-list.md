---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 018c75851a176cc1350933a8dd32c8ef0739fe41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685571"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="e9ca3-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e9ca3-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="e9ca3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9ca3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9ca3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9ca3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9ca3-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e9ca3-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9ca3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9ca3-108">Prerequisites</span></span>
<span data-ttu-id="e9ca3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9ca3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9ca3-111">Permission type</span></span>|<span data-ttu-id="e9ca3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9ca3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9ca3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9ca3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9ca3-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ca3-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e9ca3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9ca3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9ca3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-116">Not supported.</span></span>|
|<span data-ttu-id="e9ca3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9ca3-117">Application</span></span>|<span data-ttu-id="e9ca3-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ca3-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9ca3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9ca3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e9ca3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9ca3-120">Request headers</span></span>
|<span data-ttu-id="e9ca3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9ca3-121">Header</span></span>|<span data-ttu-id="e9ca3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9ca3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9ca3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9ca3-123">Authorization</span></span>|<span data-ttu-id="e9ca3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9ca3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9ca3-125">Accept</span></span>|<span data-ttu-id="e9ca3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9ca3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9ca3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9ca3-127">Request body</span></span>
<span data-ttu-id="e9ca3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9ca3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9ca3-129">Response</span></span>
<span data-ttu-id="e9ca3-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9ca3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9ca3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9ca3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9ca3-132">Request</span></span>
<span data-ttu-id="e9ca3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="e9ca3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9ca3-134">Response</span></span>
<span data-ttu-id="e9ca3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9ca3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





