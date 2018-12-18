---
title: Функция getEffectivePermissions
description: Н/Д
author: tfitzmac
ms.openlocfilehash: a4e188e9d8ec098f66274e9dbeecb852bb34914b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317859"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="05091-103">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="05091-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="05091-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05091-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05091-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05091-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05091-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05091-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05091-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05091-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05091-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="05091-108">Prerequisites</span></span>
<span data-ttu-id="05091-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05091-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05091-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05091-111">Permission type</span></span>|<span data-ttu-id="05091-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05091-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05091-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05091-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05091-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="05091-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="05091-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="05091-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="05091-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05091-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05091-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05091-117">Not supported.</span></span>|
|<span data-ttu-id="05091-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05091-118">Application</span></span>|<span data-ttu-id="05091-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05091-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05091-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05091-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="05091-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05091-121">Request headers</span></span>
|<span data-ttu-id="05091-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05091-122">Header</span></span>|<span data-ttu-id="05091-123">Значение</span><span class="sxs-lookup"><span data-stu-id="05091-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05091-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05091-124">Authorization</span></span>|<span data-ttu-id="05091-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05091-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05091-126">Accept</span><span class="sxs-lookup"><span data-stu-id="05091-126">Accept</span></span>|<span data-ttu-id="05091-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05091-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05091-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05091-128">Request body</span></span>
<span data-ttu-id="05091-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="05091-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="05091-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="05091-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="05091-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="05091-131">Property</span></span>|<span data-ttu-id="05091-132">Тип</span><span class="sxs-lookup"><span data-stu-id="05091-132">Type</span></span>|<span data-ttu-id="05091-133">Описание</span><span class="sxs-lookup"><span data-stu-id="05091-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05091-134">scope</span><span class="sxs-lookup"><span data-stu-id="05091-134">scope</span></span>|<span data-ttu-id="05091-135">Строка</span><span class="sxs-lookup"><span data-stu-id="05091-135">String</span></span>|<span data-ttu-id="05091-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05091-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05091-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="05091-137">Response</span></span>
<span data-ttu-id="05091-138">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune-rbac-rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05091-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05091-139">Пример</span><span class="sxs-lookup"><span data-stu-id="05091-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="05091-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="05091-140">Request</span></span>
<span data-ttu-id="05091-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05091-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="05091-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="05091-142">Response</span></span>
<span data-ttu-id="05091-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05091-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



