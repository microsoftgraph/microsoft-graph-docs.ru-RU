---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59da2a86d176890b50e47c0ef6743aa517d4c3af
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250945"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="88108-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="88108-103">List roleDefinitions</span></span>

> <span data-ttu-id="88108-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88108-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88108-105">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="88108-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88108-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="88108-106">Prerequisites</span></span>
<span data-ttu-id="88108-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88108-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88108-109">Permission type</span></span>|<span data-ttu-id="88108-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88108-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88108-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88108-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88108-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="88108-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="88108-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88108-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88108-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88108-114">Not supported.</span></span>|
|<span data-ttu-id="88108-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88108-115">Application</span></span>|<span data-ttu-id="88108-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88108-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88108-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88108-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="88108-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88108-118">Request headers</span></span>
|<span data-ttu-id="88108-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88108-119">Header</span></span>|<span data-ttu-id="88108-120">Значение</span><span class="sxs-lookup"><span data-stu-id="88108-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88108-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88108-121">Authorization</span></span>|<span data-ttu-id="88108-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="88108-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88108-123">Accept</span><span class="sxs-lookup"><span data-stu-id="88108-123">Accept</span></span>|<span data-ttu-id="88108-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88108-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88108-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88108-125">Request body</span></span>
<span data-ttu-id="88108-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88108-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88108-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="88108-127">Response</span></span>
<span data-ttu-id="88108-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="88108-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88108-129">Пример</span><span class="sxs-lookup"><span data-stu-id="88108-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="88108-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="88108-130">Request</span></span>
<span data-ttu-id="88108-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88108-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="88108-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="88108-132">Response</span></span>
<span data-ttu-id="88108-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88108-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



