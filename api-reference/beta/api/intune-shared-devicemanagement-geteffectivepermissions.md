---
title: Функция getEffectivePermissions
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09fe1d2e7ac473b3fc0493e634c21f8d9eaf6639
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164479"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="4f0e0-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="4f0e0-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="4f0e0-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f0e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f0e0-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f0e0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f0e0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f0e0-108">Prerequisites</span></span>
<span data-ttu-id="4f0e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="4f0e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0e0-111">Permission type</span></span>|<span data-ttu-id="4f0e0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f0e0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f0e0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4f0e0-114">&nbsp;&nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="4f0e0-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4f0e0-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f0e0-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="4f0e0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0e0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f0e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-117">Not supported.</span></span>|
|<span data-ttu-id="4f0e0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f0e0-118">Application</span></span>|<span data-ttu-id="4f0e0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f0e0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0e0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="4f0e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f0e0-121">Request headers</span></span>
|<span data-ttu-id="4f0e0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f0e0-122">Header</span></span>|<span data-ttu-id="4f0e0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4f0e0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f0e0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f0e0-124">Authorization</span></span>|<span data-ttu-id="4f0e0-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4f0e0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f0e0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4f0e0-126">Accept</span></span>|<span data-ttu-id="4f0e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4f0e0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f0e0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f0e0-128">Request body</span></span>
<span data-ttu-id="4f0e0-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4f0e0-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4f0e0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f0e0-131">Property</span></span>|<span data-ttu-id="4f0e0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4f0e0-132">Type</span></span>|<span data-ttu-id="4f0e0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0e0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f0e0-134">scope</span><span class="sxs-lookup"><span data-stu-id="4f0e0-134">scope</span></span>|<span data-ttu-id="4f0e0-135">String</span><span class="sxs-lookup"><span data-stu-id="4f0e0-135">String</span></span>|<span data-ttu-id="4f0e0-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4f0e0-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f0e0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0e0-137">Response</span></span>
<span data-ttu-id="4f0e0-138">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f0e0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0e0-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f0e0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0e0-140">Request</span></span>
<span data-ttu-id="4f0e0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4f0e0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f0e0-142">Response</span></span>
<span data-ttu-id="4f0e0-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f0e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



