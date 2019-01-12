---
title: Функция getEffectivePermissions
description: Получает действующие разрешения пользователя, прошедшего проверку подлинности
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f40412a8d95fd6bde17843b0c13e81f00459dd12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980078"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="c0b2f-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="c0b2f-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="c0b2f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0b2f-105">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="c0b2f-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0b2f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0b2f-106">Prerequisites</span></span>
<span data-ttu-id="c0b2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b2f-109">Permission type</span></span>|<span data-ttu-id="c0b2f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0b2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0b2f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c0b2f-112">&nbsp;&nbsp; Управления доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="c0b2f-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="c0b2f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0b2f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c0b2f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0b2f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b2f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-115">Not supported.</span></span>|
|<span data-ttu-id="c0b2f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0b2f-116">Application</span></span>|<span data-ttu-id="c0b2f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b2f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0b2f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="c0b2f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0b2f-119">Request headers</span></span>
|<span data-ttu-id="c0b2f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0b2f-120">Header</span></span>|<span data-ttu-id="c0b2f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c0b2f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b2f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b2f-122">Authorization</span></span>|<span data-ttu-id="c0b2f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c0b2f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b2f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c0b2f-124">Accept</span></span>|<span data-ttu-id="c0b2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b2f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b2f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0b2f-126">Request body</span></span>
<span data-ttu-id="c0b2f-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c0b2f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c0b2f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0b2f-129">Property</span></span>|<span data-ttu-id="c0b2f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c0b2f-130">Type</span></span>|<span data-ttu-id="c0b2f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c0b2f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b2f-132">scope</span><span class="sxs-lookup"><span data-stu-id="c0b2f-132">scope</span></span>|<span data-ttu-id="c0b2f-133">String</span><span class="sxs-lookup"><span data-stu-id="c0b2f-133">String</span></span>|<span data-ttu-id="c0b2f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0b2f-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="c0b2f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0b2f-135">Response</span></span>
<span data-ttu-id="c0b2f-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b2f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c0b2f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0b2f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0b2f-138">Request</span></span>
<span data-ttu-id="c0b2f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c0b2f-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0b2f-140">Response</span></span>
<span data-ttu-id="c0b2f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



