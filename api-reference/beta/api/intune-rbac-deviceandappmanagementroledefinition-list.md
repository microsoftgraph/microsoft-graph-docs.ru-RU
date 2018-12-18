---
title: Перечисление объектов deviceAndAppManagementRoleDefinition
description: Список свойств и связей объектов deviceAndAppManagementRoleDefinition.
author: tfitzmac
ms.openlocfilehash: 5705afa2faa02ad76cd9f9a7b429944d90275c72
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321317"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="d5c29-103">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5c29-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="d5c29-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5c29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5c29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5c29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5c29-107">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d5c29-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5c29-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5c29-108">Prerequisites</span></span>
<span data-ttu-id="d5c29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5c29-111">Permission type</span></span>|<span data-ttu-id="d5c29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5c29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c29-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c29-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d5c29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c29-116">Not supported.</span></span>|
|<span data-ttu-id="d5c29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5c29-117">Application</span></span>|<span data-ttu-id="d5c29-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="d5c29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5c29-120">Request headers</span></span>
|<span data-ttu-id="d5c29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5c29-121">Header</span></span>|<span data-ttu-id="d5c29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5c29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5c29-123">Authorization</span></span>|<span data-ttu-id="d5c29-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d5c29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c29-125">Accept</span></span>|<span data-ttu-id="d5c29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5c29-127">Request body</span></span>
<span data-ttu-id="d5c29-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5c29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c29-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5c29-129">Response</span></span>
<span data-ttu-id="d5c29-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5c29-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d5c29-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5c29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5c29-132">Request</span></span>
<span data-ttu-id="d5c29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5c29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="d5c29-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5c29-134">Response</span></span>
<span data-ttu-id="d5c29-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d5c29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1425

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
      "isBuiltIn": true
    }
  ]
}
```





