---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bed8a2fd1baf8396bd49801a9bbfb41276bda9e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732793"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="46b1b-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="46b1b-103">getEffectivePermissions function</span></span>

<span data-ttu-id="46b1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46b1b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46b1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46b1b-106">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="46b1b-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46b1b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46b1b-107">Prerequisites</span></span>
<span data-ttu-id="46b1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46b1b-110">Permission type</span></span>|<span data-ttu-id="46b1b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46b1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46b1b-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="46b1b-113">&nbsp;&nbsp;Управление доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="46b1b-113">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="46b1b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="46b1b-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="46b1b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46b1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b1b-116">Not supported.</span></span>|
|<span data-ttu-id="46b1b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46b1b-117">Application</span></span>|<span data-ttu-id="46b1b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b1b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46b1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="46b1b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46b1b-120">Request headers</span></span>
|<span data-ttu-id="46b1b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46b1b-121">Header</span></span>|<span data-ttu-id="46b1b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46b1b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46b1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b1b-123">Authorization</span></span>|<span data-ttu-id="46b1b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46b1b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46b1b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46b1b-125">Accept</span></span>|<span data-ttu-id="46b1b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46b1b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b1b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46b1b-127">Request body</span></span>
<span data-ttu-id="46b1b-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="46b1b-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="46b1b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="46b1b-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="46b1b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46b1b-130">Property</span></span>|<span data-ttu-id="46b1b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46b1b-131">Type</span></span>|<span data-ttu-id="46b1b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46b1b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b1b-133">scope</span><span class="sxs-lookup"><span data-stu-id="46b1b-133">scope</span></span>|<span data-ttu-id="46b1b-134">String</span><span class="sxs-lookup"><span data-stu-id="46b1b-134">String</span></span>|<span data-ttu-id="46b1b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="46b1b-135">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="46b1b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="46b1b-136">Response</span></span>
<span data-ttu-id="46b1b-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46b1b-137">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b1b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="46b1b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="46b1b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="46b1b-139">Request</span></span>
<span data-ttu-id="46b1b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46b1b-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="46b1b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="46b1b-141">Response</span></span>
<span data-ttu-id="46b1b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46b1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









