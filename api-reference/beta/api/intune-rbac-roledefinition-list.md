---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44376ea38bf460eff88451a80c328b9a9134c06e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801630"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="7ac1f-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ac1f-103">List roleDefinitions</span></span>

> <span data-ttu-id="7ac1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac1f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac1f-106">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac1f-106">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac1f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ac1f-107">Prerequisites</span></span>
<span data-ttu-id="7ac1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ac1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ac1f-110">Permission type</span></span>|<span data-ttu-id="7ac1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ac1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ac1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac1f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ac1f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7ac1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ac1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-115">Not supported.</span></span>|
|<span data-ttu-id="7ac1f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ac1f-116">Application</span></span>|<span data-ttu-id="7ac1f-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ac1f-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ac1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7ac1f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ac1f-119">Request headers</span></span>
|<span data-ttu-id="7ac1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ac1f-120">Header</span></span>|<span data-ttu-id="7ac1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7ac1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac1f-122">Authorization</span></span>|<span data-ttu-id="7ac1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7ac1f-124">Accept</span></span>|<span data-ttu-id="7ac1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac1f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ac1f-126">Request body</span></span>
<span data-ttu-id="7ac1f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ac1f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ac1f-128">Response</span></span>
<span data-ttu-id="7ac1f-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-129">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac1f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7ac1f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac1f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ac1f-131">Request</span></span>
<span data-ttu-id="7ac1f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7ac1f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ac1f-133">Response</span></span>
<span data-ttu-id="7ac1f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ac1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleDefinition",
      "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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




