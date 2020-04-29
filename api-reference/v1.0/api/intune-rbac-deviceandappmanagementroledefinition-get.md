---
title: Получение deviceAndAppManagementRoleDefinition
description: Считывание свойств и связей объекта deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd246d1b45735c9334de0025dc82cf034e8e3b45
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452656"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="24dbf-103">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="24dbf-103">Get deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="24dbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24dbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24dbf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24dbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24dbf-106">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="24dbf-106">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24dbf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24dbf-107">Prerequisites</span></span>
<span data-ttu-id="24dbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24dbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24dbf-110">Permission type</span></span>|<span data-ttu-id="24dbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24dbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24dbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24dbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24dbf-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="24dbf-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="24dbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24dbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24dbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24dbf-115">Not supported.</span></span>|
|<span data-ttu-id="24dbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24dbf-116">Application</span></span>|<span data-ttu-id="24dbf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24dbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24dbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24dbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24dbf-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24dbf-119">Optional query parameters</span></span>
<span data-ttu-id="24dbf-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="24dbf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24dbf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24dbf-121">Request headers</span></span>
|<span data-ttu-id="24dbf-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24dbf-122">Header</span></span>|<span data-ttu-id="24dbf-123">Значение</span><span class="sxs-lookup"><span data-stu-id="24dbf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24dbf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24dbf-124">Authorization</span></span>|<span data-ttu-id="24dbf-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24dbf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24dbf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="24dbf-126">Accept</span></span>|<span data-ttu-id="24dbf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24dbf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24dbf-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24dbf-128">Request body</span></span>
<span data-ttu-id="24dbf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24dbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24dbf-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="24dbf-130">Response</span></span>
<span data-ttu-id="24dbf-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24dbf-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24dbf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="24dbf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24dbf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24dbf-133">Request</span></span>
<span data-ttu-id="24dbf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24dbf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="24dbf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="24dbf-135">Response</span></span>
<span data-ttu-id="24dbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24dbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```






