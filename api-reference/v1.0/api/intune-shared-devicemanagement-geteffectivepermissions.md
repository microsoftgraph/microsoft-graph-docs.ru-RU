---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3609bb419b9fc7bf39074827915717428224443b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025888"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="aadbe-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="aadbe-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="aadbe-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aadbe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aadbe-105">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="aadbe-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aadbe-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aadbe-106">Prerequisites</span></span>
<span data-ttu-id="aadbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aadbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aadbe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aadbe-109">Permission type</span></span>|<span data-ttu-id="aadbe-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aadbe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aadbe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aadbe-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aadbe-112">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="aadbe-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="aadbe-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aadbe-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="aadbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aadbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aadbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aadbe-115">Not supported.</span></span>|
|<span data-ttu-id="aadbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aadbe-116">Application</span></span>|<span data-ttu-id="aadbe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aadbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aadbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aadbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="aadbe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aadbe-119">Request headers</span></span>
|<span data-ttu-id="aadbe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aadbe-120">Header</span></span>|<span data-ttu-id="aadbe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aadbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aadbe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aadbe-122">Authorization</span></span>|<span data-ttu-id="aadbe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aadbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aadbe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aadbe-124">Accept</span></span>|<span data-ttu-id="aadbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aadbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aadbe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aadbe-126">Request body</span></span>
<span data-ttu-id="aadbe-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="aadbe-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="aadbe-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="aadbe-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="aadbe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aadbe-129">Property</span></span>|<span data-ttu-id="aadbe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aadbe-130">Type</span></span>|<span data-ttu-id="aadbe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aadbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aadbe-132">scope</span><span class="sxs-lookup"><span data-stu-id="aadbe-132">scope</span></span>|<span data-ttu-id="aadbe-133">String</span><span class="sxs-lookup"><span data-stu-id="aadbe-133">String</span></span>|<span data-ttu-id="aadbe-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aadbe-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="aadbe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aadbe-135">Response</span></span>
<span data-ttu-id="aadbe-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aadbe-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aadbe-137">Пример</span><span class="sxs-lookup"><span data-stu-id="aadbe-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="aadbe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="aadbe-138">Request</span></span>
<span data-ttu-id="aadbe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aadbe-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="aadbe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="aadbe-140">Response</span></span>
<span data-ttu-id="aadbe-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aadbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



