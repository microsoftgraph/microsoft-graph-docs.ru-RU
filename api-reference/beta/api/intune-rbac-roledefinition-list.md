---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 274c3e9b9e88e4d32b81e3c1a0c6c09a48181bf0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978245"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="dbb7b-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dbb7b-103">List roleDefinitions</span></span>

> <span data-ttu-id="dbb7b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbb7b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbb7b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbb7b-107">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dbb7b-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbb7b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dbb7b-108">Prerequisites</span></span>
<span data-ttu-id="dbb7b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbb7b-111">Permission type</span></span>|<span data-ttu-id="dbb7b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbb7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbb7b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbb7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbb7b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbb7b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="dbb7b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbb7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbb7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-116">Not supported.</span></span>|
|<span data-ttu-id="dbb7b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbb7b-117">Application</span></span>|<span data-ttu-id="dbb7b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbb7b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbb7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="dbb7b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbb7b-120">Request headers</span></span>
|<span data-ttu-id="dbb7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbb7b-121">Header</span></span>|<span data-ttu-id="dbb7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dbb7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbb7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbb7b-123">Authorization</span></span>|<span data-ttu-id="dbb7b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dbb7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbb7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dbb7b-125">Accept</span></span>|<span data-ttu-id="dbb7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbb7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb7b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbb7b-127">Request body</span></span>
<span data-ttu-id="dbb7b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbb7b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbb7b-129">Response</span></span>
<span data-ttu-id="dbb7b-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbb7b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dbb7b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbb7b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbb7b-132">Request</span></span>
<span data-ttu-id="dbb7b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="dbb7b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbb7b-134">Response</span></span>
<span data-ttu-id="dbb7b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dbb7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

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
      "isBuiltIn": true
    }
  ]
}
```





