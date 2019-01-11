---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97919fd8a4fc61da2c54cdd53ebbdd19e20eafc3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806232"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="0d880-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0d880-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="0d880-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d880-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d880-105">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0d880-105">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d880-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d880-106">Prerequisites</span></span>
<span data-ttu-id="0d880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d880-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d880-109">Permission type</span></span>|<span data-ttu-id="0d880-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d880-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d880-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d880-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d880-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d880-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0d880-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d880-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d880-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d880-114">Not supported.</span></span>|
|<span data-ttu-id="0d880-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d880-115">Application</span></span>|<span data-ttu-id="0d880-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d880-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d880-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d880-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="0d880-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d880-118">Request headers</span></span>
|<span data-ttu-id="0d880-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d880-119">Header</span></span>|<span data-ttu-id="0d880-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0d880-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d880-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d880-121">Authorization</span></span>|<span data-ttu-id="0d880-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d880-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d880-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0d880-123">Accept</span></span>|<span data-ttu-id="0d880-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0d880-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d880-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d880-125">Request body</span></span>
<span data-ttu-id="0d880-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d880-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d880-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d880-127">Response</span></span>
<span data-ttu-id="0d880-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d880-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d880-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0d880-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d880-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d880-130">Request</span></span>
<span data-ttu-id="0d880-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d880-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="0d880-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d880-132">Response</span></span>
<span data-ttu-id="0d880-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d880-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



