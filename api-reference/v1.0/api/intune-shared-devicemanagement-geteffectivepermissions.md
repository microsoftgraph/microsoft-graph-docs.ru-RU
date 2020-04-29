---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26bc43b1dbd7e82133ad4ff54b7b9ba1bbf855bd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463838"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="d78a4-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="d78a4-103">getEffectivePermissions function</span></span>

<span data-ttu-id="d78a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d78a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d78a4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d78a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78a4-106">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="d78a4-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d78a4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d78a4-107">Prerequisites</span></span>
<span data-ttu-id="d78a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d78a4-110">Permission type</span></span>|<span data-ttu-id="d78a4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d78a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d78a4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d78a4-113">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="d78a4-113">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="d78a4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d78a4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d78a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d78a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78a4-116">Not supported.</span></span>|
|<span data-ttu-id="d78a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d78a4-117">Application</span></span>|<span data-ttu-id="d78a4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d78a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="d78a4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d78a4-120">Request headers</span></span>
|<span data-ttu-id="d78a4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d78a4-121">Header</span></span>|<span data-ttu-id="d78a4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d78a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78a4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d78a4-123">Authorization</span></span>|<span data-ttu-id="d78a4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d78a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d78a4-125">Accept</span></span>|<span data-ttu-id="d78a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d78a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78a4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d78a4-127">Request body</span></span>
<span data-ttu-id="d78a4-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d78a4-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d78a4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="d78a4-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d78a4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d78a4-130">Property</span></span>|<span data-ttu-id="d78a4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d78a4-131">Type</span></span>|<span data-ttu-id="d78a4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d78a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78a4-133">scope</span><span class="sxs-lookup"><span data-stu-id="d78a4-133">scope</span></span>|<span data-ttu-id="d78a4-134">String</span><span class="sxs-lookup"><span data-stu-id="d78a4-134">String</span></span>|<span data-ttu-id="d78a4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d78a4-135">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="d78a4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78a4-136">Response</span></span>
<span data-ttu-id="d78a4-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d78a4-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78a4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d78a4-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="d78a4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d78a4-139">Request</span></span>
<span data-ttu-id="d78a4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d78a4-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d78a4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78a4-141">Response</span></span>
<span data-ttu-id="d78a4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d78a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
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
  ]
}
```






