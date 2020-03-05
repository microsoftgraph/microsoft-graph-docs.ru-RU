---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab0df9a407715651ecb3c3ce567da3a428c81c50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459683"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="fbf73-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fbf73-103">List roleDefinitions</span></span>

<span data-ttu-id="fbf73-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fbf73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbf73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbf73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf73-107">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fbf73-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbf73-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fbf73-108">Prerequisites</span></span>
<span data-ttu-id="fbf73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbf73-111">Permission type</span></span>|<span data-ttu-id="fbf73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbf73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbf73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf73-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbf73-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fbf73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbf73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf73-116">Not supported.</span></span>|
|<span data-ttu-id="fbf73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbf73-117">Application</span></span>|<span data-ttu-id="fbf73-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbf73-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbf73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="fbf73-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbf73-120">Request headers</span></span>
|<span data-ttu-id="fbf73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbf73-121">Header</span></span>|<span data-ttu-id="fbf73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbf73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf73-123">Authorization</span></span>|<span data-ttu-id="fbf73-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbf73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbf73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbf73-125">Accept</span></span>|<span data-ttu-id="fbf73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf73-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbf73-127">Request body</span></span>
<span data-ttu-id="fbf73-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbf73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf73-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbf73-129">Response</span></span>
<span data-ttu-id="fbf73-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbf73-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf73-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fbf73-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbf73-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbf73-132">Request</span></span>
<span data-ttu-id="fbf73-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbf73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="fbf73-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbf73-134">Response</span></span>
<span data-ttu-id="fbf73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbf73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





