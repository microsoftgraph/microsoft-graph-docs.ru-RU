---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d03ab6dd6633de58df090710e1ecae7bb216804
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512071"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="a5458-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="a5458-103">getEffectivePermissions function</span></span>

<span data-ttu-id="a5458-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5458-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5458-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5458-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5458-106">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="a5458-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5458-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5458-107">Prerequisites</span></span>
<span data-ttu-id="a5458-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5458-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5458-110">Permission type</span></span>|<span data-ttu-id="a5458-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5458-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5458-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5458-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a5458-113">&nbsp;&nbsp; Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="a5458-113">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="a5458-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5458-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a5458-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5458-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5458-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5458-116">Not supported.</span></span>|
|<span data-ttu-id="a5458-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5458-117">Application</span></span>|<span data-ttu-id="a5458-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5458-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5458-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5458-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="a5458-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5458-120">Request headers</span></span>
|<span data-ttu-id="a5458-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5458-121">Header</span></span>|<span data-ttu-id="a5458-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5458-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5458-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5458-123">Authorization</span></span>|<span data-ttu-id="a5458-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5458-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5458-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5458-125">Accept</span></span>|<span data-ttu-id="a5458-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5458-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5458-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5458-127">Request body</span></span>
<span data-ttu-id="a5458-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a5458-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a5458-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a5458-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a5458-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5458-130">Property</span></span>|<span data-ttu-id="a5458-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5458-131">Type</span></span>|<span data-ttu-id="a5458-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5458-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5458-133">scope</span><span class="sxs-lookup"><span data-stu-id="a5458-133">scope</span></span>|<span data-ttu-id="a5458-134">String</span><span class="sxs-lookup"><span data-stu-id="a5458-134">String</span></span>|<span data-ttu-id="a5458-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5458-135">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="a5458-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5458-136">Response</span></span>
<span data-ttu-id="a5458-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5458-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5458-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a5458-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5458-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5458-139">Request</span></span>
<span data-ttu-id="a5458-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5458-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a5458-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5458-141">Response</span></span>
<span data-ttu-id="a5458-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5458-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




