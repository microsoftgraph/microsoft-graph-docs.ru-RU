---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd1d98d35d5fff7232b018dd12d1262cf477a34a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512295"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="68c4e-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="68c4e-103">List deviceAndAppManagementRoleDefinitions</span></span>

<span data-ttu-id="68c4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68c4e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68c4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c4e-106">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="68c4e-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68c4e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68c4e-107">Prerequisites</span></span>
<span data-ttu-id="68c4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c4e-110">Permission type</span></span>|<span data-ttu-id="68c4e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68c4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68c4e-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="68c4e-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="68c4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68c4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c4e-115">Not supported.</span></span>|
|<span data-ttu-id="68c4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68c4e-116">Application</span></span>|<span data-ttu-id="68c4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68c4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="68c4e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68c4e-119">Request headers</span></span>
|<span data-ttu-id="68c4e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68c4e-120">Header</span></span>|<span data-ttu-id="68c4e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68c4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68c4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68c4e-122">Authorization</span></span>|<span data-ttu-id="68c4e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68c4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68c4e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68c4e-124">Accept</span></span>|<span data-ttu-id="68c4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68c4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68c4e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68c4e-126">Request body</span></span>
<span data-ttu-id="68c4e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68c4e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68c4e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="68c4e-128">Response</span></span>
<span data-ttu-id="68c4e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68c4e-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68c4e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="68c4e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="68c4e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c4e-131">Request</span></span>
<span data-ttu-id="68c4e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c4e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="68c4e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c4e-133">Response</span></span>
<span data-ttu-id="68c4e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




