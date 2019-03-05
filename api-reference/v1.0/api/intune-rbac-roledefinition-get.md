---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a18d199c0814d3b82fb75646fb99adc488dbfa33
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257717"
---
# <a name="get-roledefinition"></a><span data-ttu-id="fb7f0-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fb7f0-103">Get roleDefinition</span></span>

> <span data-ttu-id="fb7f0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb7f0-105">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fb7f0-105">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb7f0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fb7f0-106">Prerequisites</span></span>
<span data-ttu-id="fb7f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb7f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb7f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb7f0-109">Permission type</span></span>|<span data-ttu-id="fb7f0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb7f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb7f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb7f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb7f0-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7f0-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fb7f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb7f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb7f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-114">Not supported.</span></span>|
|<span data-ttu-id="fb7f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb7f0-115">Application</span></span>|<span data-ttu-id="fb7f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb7f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb7f0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb7f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb7f0-118">Optional query parameters</span></span>
<span data-ttu-id="fb7f0-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb7f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb7f0-120">Request headers</span></span>
|<span data-ttu-id="fb7f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb7f0-121">Header</span></span>|<span data-ttu-id="fb7f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb7f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb7f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb7f0-123">Authorization</span></span>|<span data-ttu-id="fb7f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb7f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb7f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb7f0-125">Accept</span></span>|<span data-ttu-id="fb7f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb7f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb7f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb7f0-127">Request body</span></span>
<span data-ttu-id="fb7f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb7f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb7f0-129">Response</span></span>
<span data-ttu-id="fb7f0-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-130">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb7f0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fb7f0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb7f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb7f0-132">Request</span></span>
<span data-ttu-id="fb7f0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="fb7f0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb7f0-134">Response</span></span>
<span data-ttu-id="fb7f0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb7f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



