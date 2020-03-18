---
title: Функция getEffectivePermissions
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e480b90dba719f52d49c4afb8fc2646be7d4660
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801063"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="fd864-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="fd864-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="fd864-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd864-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd864-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd864-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd864-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd864-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd864-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fd864-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd864-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd864-108">Prerequisites</span></span>
<span data-ttu-id="fd864-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd864-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd864-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd864-111">Permission type</span></span>|<span data-ttu-id="fd864-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd864-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd864-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd864-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fd864-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="fd864-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="fd864-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd864-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fd864-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd864-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd864-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd864-117">Not supported.</span></span>|
|<span data-ttu-id="fd864-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="fd864-118">Application</span></span>||
| <span data-ttu-id="fd864-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="fd864-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="fd864-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd864-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd864-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd864-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="fd864-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fd864-122">Request headers</span></span>
|<span data-ttu-id="fd864-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd864-123">Header</span></span>|<span data-ttu-id="fd864-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fd864-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd864-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd864-125">Authorization</span></span>|<span data-ttu-id="fd864-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd864-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd864-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fd864-127">Accept</span></span>|<span data-ttu-id="fd864-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fd864-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd864-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd864-129">Request body</span></span>
<span data-ttu-id="fd864-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fd864-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fd864-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fd864-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fd864-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd864-132">Property</span></span>|<span data-ttu-id="fd864-133">Тип</span><span class="sxs-lookup"><span data-stu-id="fd864-133">Type</span></span>|<span data-ttu-id="fd864-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fd864-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd864-135">scope</span><span class="sxs-lookup"><span data-stu-id="fd864-135">scope</span></span>|<span data-ttu-id="fd864-136">String</span><span class="sxs-lookup"><span data-stu-id="fd864-136">String</span></span>|<span data-ttu-id="fd864-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fd864-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fd864-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd864-138">Response</span></span>
<span data-ttu-id="fd864-139">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd864-139">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd864-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fd864-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd864-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd864-141">Request</span></span>
<span data-ttu-id="fd864-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd864-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fd864-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd864-143">Response</span></span>
<span data-ttu-id="fd864-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd864-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










