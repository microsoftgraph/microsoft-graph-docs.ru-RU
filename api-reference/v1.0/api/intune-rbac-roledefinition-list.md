---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0cfe82cb25a939532f3900c2f37efa7070284f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965808"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="a61e8-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a61e8-103">List roleDefinitions</span></span>

<span data-ttu-id="a61e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a61e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a61e8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a61e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a61e8-106">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a61e8-106">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a61e8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a61e8-107">Prerequisites</span></span>
<span data-ttu-id="a61e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a61e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a61e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a61e8-110">Permission type</span></span>|<span data-ttu-id="a61e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a61e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a61e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a61e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a61e8-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a61e8-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a61e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a61e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a61e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a61e8-115">Not supported.</span></span>|
|<span data-ttu-id="a61e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a61e8-116">Application</span></span>|<span data-ttu-id="a61e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a61e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a61e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a61e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a61e8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a61e8-119">Request headers</span></span>
|<span data-ttu-id="a61e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a61e8-120">Header</span></span>|<span data-ttu-id="a61e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a61e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a61e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a61e8-122">Authorization</span></span>|<span data-ttu-id="a61e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a61e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a61e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a61e8-124">Accept</span></span>|<span data-ttu-id="a61e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a61e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a61e8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a61e8-126">Request body</span></span>
<span data-ttu-id="a61e8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a61e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a61e8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a61e8-128">Response</span></span>
<span data-ttu-id="a61e8-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a61e8-129">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a61e8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a61e8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a61e8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a61e8-131">Request</span></span>
<span data-ttu-id="a61e8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a61e8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="a61e8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a61e8-133">Response</span></span>
<span data-ttu-id="a61e8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a61e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









