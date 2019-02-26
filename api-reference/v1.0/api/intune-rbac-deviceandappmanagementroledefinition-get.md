---
title: Получение deviceAndAppManagementRoleDefinition
description: Считывание свойств и связей объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cb7fee4b48aab340ba248ab00fea41ae17ba41b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252177"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="cadca-103">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cadca-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="cadca-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cadca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cadca-105">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cadca-105">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cadca-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cadca-106">Prerequisites</span></span>
<span data-ttu-id="cadca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cadca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cadca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cadca-109">Permission type</span></span>|<span data-ttu-id="cadca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cadca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cadca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cadca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cadca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cadca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="cadca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cadca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cadca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cadca-114">Not supported.</span></span>|
|<span data-ttu-id="cadca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cadca-115">Application</span></span>|<span data-ttu-id="cadca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cadca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cadca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cadca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cadca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cadca-118">Optional query parameters</span></span>
<span data-ttu-id="cadca-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cadca-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cadca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cadca-120">Request headers</span></span>
|<span data-ttu-id="cadca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cadca-121">Header</span></span>|<span data-ttu-id="cadca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cadca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cadca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cadca-123">Authorization</span></span>|<span data-ttu-id="cadca-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cadca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cadca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cadca-125">Accept</span></span>|<span data-ttu-id="cadca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cadca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cadca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cadca-127">Request body</span></span>
<span data-ttu-id="cadca-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cadca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cadca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cadca-129">Response</span></span>
<span data-ttu-id="cadca-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cadca-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cadca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cadca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cadca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cadca-132">Request</span></span>
<span data-ttu-id="cadca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cadca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="cadca-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cadca-134">Response</span></span>
<span data-ttu-id="cadca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cadca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



