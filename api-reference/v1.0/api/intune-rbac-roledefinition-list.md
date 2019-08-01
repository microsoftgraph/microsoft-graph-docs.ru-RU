---
title: Перечисление объектов roleDefinition
description: Список свойств и связей объектов roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f546f100551b93749adc7625bb37f6e297e89dc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023701"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="9cc4d-103">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9cc4d-103">List roleDefinitions</span></span>

> <span data-ttu-id="9cc4d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cc4d-105">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9cc4d-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cc4d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9cc4d-106">Prerequisites</span></span>
<span data-ttu-id="9cc4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cc4d-109">Permission type</span></span>|<span data-ttu-id="9cc4d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cc4d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cc4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc4d-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc4d-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9cc4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cc4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-114">Not supported.</span></span>|
|<span data-ttu-id="9cc4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cc4d-115">Application</span></span>|<span data-ttu-id="9cc4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cc4d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9cc4d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cc4d-118">Request headers</span></span>
|<span data-ttu-id="9cc4d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cc4d-119">Header</span></span>|<span data-ttu-id="9cc4d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9cc4d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc4d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cc4d-121">Authorization</span></span>|<span data-ttu-id="9cc4d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc4d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9cc4d-123">Accept</span></span>|<span data-ttu-id="9cc4d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc4d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc4d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9cc4d-125">Request body</span></span>
<span data-ttu-id="9cc4d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cc4d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cc4d-127">Response</span></span>
<span data-ttu-id="9cc4d-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc4d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9cc4d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cc4d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cc4d-130">Request</span></span>
<span data-ttu-id="9cc4d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="9cc4d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc4d-132">Response</span></span>
<span data-ttu-id="9cc4d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cc4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



