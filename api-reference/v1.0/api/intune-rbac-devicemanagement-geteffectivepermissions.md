---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0bb5dbb4726d6818f0a144458c1239085dbe462
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757621"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="cbf84-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="cbf84-103">getEffectivePermissions function</span></span>

<span data-ttu-id="cbf84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbf84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbf84-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbf84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbf84-106">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="cbf84-106">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbf84-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cbf84-107">Prerequisites</span></span>
<span data-ttu-id="cbf84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbf84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbf84-110">Permission type</span></span>|<span data-ttu-id="cbf84-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbf84-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbf84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbf84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbf84-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbf84-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cbf84-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbf84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbf84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbf84-115">Not supported.</span></span>|
|<span data-ttu-id="cbf84-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cbf84-116">Application</span></span>|<span data-ttu-id="cbf84-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbf84-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbf84-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbf84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="cbf84-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cbf84-119">Request headers</span></span>
|<span data-ttu-id="cbf84-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbf84-120">Header</span></span>|<span data-ttu-id="cbf84-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cbf84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbf84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbf84-122">Authorization</span></span>|<span data-ttu-id="cbf84-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbf84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbf84-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cbf84-124">Accept</span></span>|<span data-ttu-id="cbf84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbf84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf84-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbf84-126">Request body</span></span>
<span data-ttu-id="cbf84-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="cbf84-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cbf84-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="cbf84-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cbf84-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbf84-129">Property</span></span>|<span data-ttu-id="cbf84-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cbf84-130">Type</span></span>|<span data-ttu-id="cbf84-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cbf84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbf84-132">scope</span><span class="sxs-lookup"><span data-stu-id="cbf84-132">scope</span></span>|<span data-ttu-id="cbf84-133">String</span><span class="sxs-lookup"><span data-stu-id="cbf84-133">String</span></span>|<span data-ttu-id="cbf84-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cbf84-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbf84-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf84-135">Response</span></span>
<span data-ttu-id="cbf84-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cbf84-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf84-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cbf84-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbf84-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbf84-138">Request</span></span>
<span data-ttu-id="cbf84-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbf84-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cbf84-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf84-140">Response</span></span>
<span data-ttu-id="cbf84-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbf84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
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
  ]
}
```




