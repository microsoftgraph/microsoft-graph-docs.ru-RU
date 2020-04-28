---
title: Функция getEffectivePermissions
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ec8e3bf80ea0e9fb7077f3bac2d7bcf97c217d5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390170"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="91589-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="91589-103">getEffectivePermissions function</span></span>

<span data-ttu-id="91589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91589-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91589-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91589-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91589-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91589-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91589-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91589-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="91589-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91589-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91589-109">Prerequisites</span></span>
<span data-ttu-id="91589-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91589-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91589-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91589-112">Permission type</span></span>|<span data-ttu-id="91589-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91589-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91589-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91589-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="91589-115">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="91589-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="91589-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="91589-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="91589-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91589-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91589-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91589-118">Not supported.</span></span>|
|<span data-ttu-id="91589-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91589-119">Application</span></span>||
| <span data-ttu-id="91589-120">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="91589-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="91589-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="91589-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91589-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91589-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="91589-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="91589-123">Request headers</span></span>
|<span data-ttu-id="91589-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91589-124">Header</span></span>|<span data-ttu-id="91589-125">Значение</span><span class="sxs-lookup"><span data-stu-id="91589-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91589-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91589-126">Authorization</span></span>|<span data-ttu-id="91589-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91589-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91589-128">Accept</span><span class="sxs-lookup"><span data-stu-id="91589-128">Accept</span></span>|<span data-ttu-id="91589-129">application/json</span><span class="sxs-lookup"><span data-stu-id="91589-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91589-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91589-130">Request body</span></span>
<span data-ttu-id="91589-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="91589-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="91589-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="91589-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="91589-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="91589-133">Property</span></span>|<span data-ttu-id="91589-134">Тип</span><span class="sxs-lookup"><span data-stu-id="91589-134">Type</span></span>|<span data-ttu-id="91589-135">Описание</span><span class="sxs-lookup"><span data-stu-id="91589-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91589-136">scope</span><span class="sxs-lookup"><span data-stu-id="91589-136">scope</span></span>|<span data-ttu-id="91589-137">String</span><span class="sxs-lookup"><span data-stu-id="91589-137">String</span></span>|<span data-ttu-id="91589-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="91589-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="91589-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="91589-139">Response</span></span>
<span data-ttu-id="91589-140">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91589-140">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91589-141">Пример</span><span class="sxs-lookup"><span data-stu-id="91589-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="91589-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="91589-142">Request</span></span>
<span data-ttu-id="91589-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91589-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="91589-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="91589-144">Response</span></span>
<span data-ttu-id="91589-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91589-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









