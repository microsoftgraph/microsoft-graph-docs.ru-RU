---
title: Функция getEffectivePermissions
description: Н/Д
ms.openlocfilehash: dc2f9022a0f87e3869191ecea8a65ac9d60d6c9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077390"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="de8be-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="de8be-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="de8be-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de8be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de8be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de8be-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de8be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de8be-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de8be-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de8be-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="de8be-108">Prerequisites</span></span>
<span data-ttu-id="de8be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de8be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de8be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de8be-111">Permission type</span></span>|<span data-ttu-id="de8be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de8be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de8be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de8be-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="de8be-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="de8be-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="de8be-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="de8be-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="de8be-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de8be-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de8be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8be-117">Not supported.</span></span>|
|<span data-ttu-id="de8be-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de8be-118">Application</span></span>|<span data-ttu-id="de8be-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8be-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de8be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de8be-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="de8be-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de8be-121">Request headers</span></span>
|<span data-ttu-id="de8be-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de8be-122">Header</span></span>|<span data-ttu-id="de8be-123">Значение</span><span class="sxs-lookup"><span data-stu-id="de8be-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de8be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="de8be-124">Authorization</span></span>|<span data-ttu-id="de8be-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="de8be-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de8be-126">Accept</span><span class="sxs-lookup"><span data-stu-id="de8be-126">Accept</span></span>|<span data-ttu-id="de8be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="de8be-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de8be-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de8be-128">Request body</span></span>
<span data-ttu-id="de8be-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="de8be-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="de8be-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="de8be-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="de8be-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="de8be-131">Property</span></span>|<span data-ttu-id="de8be-132">Тип</span><span class="sxs-lookup"><span data-stu-id="de8be-132">Type</span></span>|<span data-ttu-id="de8be-133">Описание</span><span class="sxs-lookup"><span data-stu-id="de8be-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8be-134">scope</span><span class="sxs-lookup"><span data-stu-id="de8be-134">scope</span></span>|<span data-ttu-id="de8be-135">String</span><span class="sxs-lookup"><span data-stu-id="de8be-135">String</span></span>|<span data-ttu-id="de8be-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de8be-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de8be-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="de8be-137">Response</span></span>
<span data-ttu-id="de8be-138">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="de8be-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de8be-139">Пример</span><span class="sxs-lookup"><span data-stu-id="de8be-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="de8be-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="de8be-140">Request</span></span>
<span data-ttu-id="de8be-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de8be-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="de8be-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="de8be-142">Response</span></span>
<span data-ttu-id="de8be-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="de8be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



