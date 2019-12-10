---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1347a32f9ec4dd8f216e8fd38600652b5089cec
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940688"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="e988d-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e988d-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="e988d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e988d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e988d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e988d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e988d-106">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e988d-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e988d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e988d-107">Prerequisites</span></span>
<span data-ttu-id="e988d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e988d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e988d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e988d-110">Permission type</span></span>|<span data-ttu-id="e988d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e988d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e988d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e988d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e988d-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e988d-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e988d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e988d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e988d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e988d-115">Not supported.</span></span>|
|<span data-ttu-id="e988d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e988d-116">Application</span></span>|<span data-ttu-id="e988d-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e988d-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e988d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e988d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e988d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e988d-119">Request headers</span></span>
|<span data-ttu-id="e988d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e988d-120">Header</span></span>|<span data-ttu-id="e988d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e988d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e988d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e988d-122">Authorization</span></span>|<span data-ttu-id="e988d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e988d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e988d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e988d-124">Accept</span></span>|<span data-ttu-id="e988d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e988d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e988d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e988d-126">Request body</span></span>
<span data-ttu-id="e988d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e988d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e988d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e988d-128">Response</span></span>
<span data-ttu-id="e988d-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e988d-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e988d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e988d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e988d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e988d-131">Request</span></span>
<span data-ttu-id="e988d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e988d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="e988d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e988d-133">Response</span></span>
<span data-ttu-id="e988d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e988d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





