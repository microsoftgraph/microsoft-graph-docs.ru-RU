---
title: функция getAssignedRoleIdsForLoggedInUser
description: Извлекает назначенной роли определения и назначения ролей текущего прошедшего проверку пользователя.
ms.openlocfilehash: c97e701bfd35961d9fb15022500bb06727c7e89a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077360"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="be592-103">функция getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="be592-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="be592-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be592-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be592-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be592-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be592-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be592-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be592-107">Извлекает назначенной роли определения и назначения ролей текущего прошедшего проверку пользователя.</span><span class="sxs-lookup"><span data-stu-id="be592-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be592-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be592-108">Prerequisites</span></span>
<span data-ttu-id="be592-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be592-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be592-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be592-111">Permission type</span></span>|<span data-ttu-id="be592-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be592-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be592-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be592-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be592-114">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="be592-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="be592-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="be592-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="be592-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be592-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be592-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be592-117">Not supported.</span></span>|
|<span data-ttu-id="be592-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be592-118">Application</span></span>|<span data-ttu-id="be592-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be592-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be592-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be592-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="be592-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be592-121">Request headers</span></span>
|<span data-ttu-id="be592-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be592-122">Header</span></span>|<span data-ttu-id="be592-123">Значение</span><span class="sxs-lookup"><span data-stu-id="be592-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be592-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be592-124">Authorization</span></span>|<span data-ttu-id="be592-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be592-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be592-126">Accept</span><span class="sxs-lookup"><span data-stu-id="be592-126">Accept</span></span>|<span data-ttu-id="be592-127">application/json</span><span class="sxs-lookup"><span data-stu-id="be592-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be592-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be592-128">Request body</span></span>
<span data-ttu-id="be592-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be592-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be592-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="be592-130">Response</span></span>
<span data-ttu-id="be592-131">Если успешно завершена, эта функция возвращает `200 OK` код ответа и [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be592-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be592-132">Пример</span><span class="sxs-lookup"><span data-stu-id="be592-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="be592-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="be592-133">Request</span></span>
<span data-ttu-id="be592-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be592-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="be592-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="be592-135">Response</span></span>
<span data-ttu-id="be592-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="be592-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```





