---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
ms.openlocfilehash: 55135d3eb48490303b66bd1839db4e05b4b3a2fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027489"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="0e2b1-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="0e2b1-103">List roleDefinitions</span></span>

> <span data-ttu-id="0e2b1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e2b1-105">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0e2b1-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e2b1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e2b1-106">Prerequisites</span></span>
<span data-ttu-id="0e2b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e2b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e2b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e2b1-109">Permission type</span></span>|<span data-ttu-id="0e2b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e2b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e2b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e2b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e2b1-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e2b1-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0e2b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e2b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e2b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-114">Not supported.</span></span>|
|<span data-ttu-id="0e2b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e2b1-115">Application</span></span>|<span data-ttu-id="0e2b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e2b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e2b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="0e2b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e2b1-118">Request headers</span></span>
|<span data-ttu-id="0e2b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e2b1-119">Header</span></span>|<span data-ttu-id="0e2b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0e2b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e2b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e2b1-121">Authorization</span></span>|<span data-ttu-id="0e2b1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e2b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e2b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0e2b1-123">Accept</span></span>|<span data-ttu-id="0e2b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e2b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e2b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e2b1-125">Request body</span></span>
<span data-ttu-id="0e2b1-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e2b1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e2b1-127">Response</span></span>
<span data-ttu-id="0e2b1-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e2b1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0e2b1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e2b1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e2b1-130">Request</span></span>
<span data-ttu-id="0e2b1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e2b1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="0e2b1-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e2b1-132">Response</span></span>
<span data-ttu-id="0e2b1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0e2b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 746

{
  "value": [
    {
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
  ]
}
```



