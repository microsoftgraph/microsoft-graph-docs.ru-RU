---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28b86dbbb15e0b900e3fa438c338978acb2ebe44
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756893"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="46fb2-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="46fb2-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="46fb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46fb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46fb2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46fb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46fb2-106">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="46fb2-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46fb2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46fb2-107">Prerequisites</span></span>
<span data-ttu-id="46fb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46fb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46fb2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46fb2-110">Permission type</span></span>|<span data-ttu-id="46fb2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46fb2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46fb2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46fb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46fb2-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46fb2-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="46fb2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46fb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46fb2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46fb2-115">Not supported.</span></span>|
|<span data-ttu-id="46fb2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="46fb2-116">Application</span></span>|<span data-ttu-id="46fb2-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46fb2-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46fb2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46fb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="46fb2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46fb2-119">Request headers</span></span>
|<span data-ttu-id="46fb2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46fb2-120">Header</span></span>|<span data-ttu-id="46fb2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46fb2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46fb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46fb2-122">Authorization</span></span>|<span data-ttu-id="46fb2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46fb2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46fb2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46fb2-124">Accept</span></span>|<span data-ttu-id="46fb2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46fb2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46fb2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46fb2-126">Request body</span></span>
<span data-ttu-id="46fb2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46fb2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46fb2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="46fb2-128">Response</span></span>
<span data-ttu-id="46fb2-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46fb2-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46fb2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="46fb2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46fb2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="46fb2-131">Request</span></span>
<span data-ttu-id="46fb2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46fb2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="46fb2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="46fb2-133">Response</span></span>
<span data-ttu-id="46fb2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46fb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
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
      "isBuiltIn": true
    }
  ]
}
```




