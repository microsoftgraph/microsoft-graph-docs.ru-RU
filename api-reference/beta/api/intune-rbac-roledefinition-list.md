---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bbc40aa61dc262b2cdfe3c73c7ad5f2ac0d90887
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304702"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="596e8-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="596e8-103">List roleDefinitions</span></span>

<span data-ttu-id="596e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="596e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="596e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="596e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="596e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="596e8-107">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="596e8-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="596e8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="596e8-108">Prerequisites</span></span>
<span data-ttu-id="596e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="596e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="596e8-111">Permission type</span></span>|<span data-ttu-id="596e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="596e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="596e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="596e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="596e8-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="596e8-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="596e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="596e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="596e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596e8-116">Not supported.</span></span>|
|<span data-ttu-id="596e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="596e8-117">Application</span></span>|<span data-ttu-id="596e8-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="596e8-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="596e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="596e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="596e8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="596e8-120">Request headers</span></span>
|<span data-ttu-id="596e8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="596e8-121">Header</span></span>|<span data-ttu-id="596e8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="596e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="596e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="596e8-123">Authorization</span></span>|<span data-ttu-id="596e8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="596e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="596e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="596e8-125">Accept</span></span>|<span data-ttu-id="596e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="596e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="596e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="596e8-127">Request body</span></span>
<span data-ttu-id="596e8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="596e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="596e8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="596e8-129">Response</span></span>
<span data-ttu-id="596e8-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="596e8-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="596e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="596e8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="596e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="596e8-132">Request</span></span>
<span data-ttu-id="596e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="596e8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="596e8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="596e8-134">Response</span></span>
<span data-ttu-id="596e8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="596e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




