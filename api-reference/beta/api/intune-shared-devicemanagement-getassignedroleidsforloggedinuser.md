---
title: Функция Жетассигнедролеидсфорлогжединусер
description: Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6790d5121c8c3eced7ee0a5ea769469b8b9eaee5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390177"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="2db66-103">Функция Жетассигнедролеидсфорлогжединусер</span><span class="sxs-lookup"><span data-stu-id="2db66-103">getAssignedRoleIdsForLoggedInUser function</span></span>

<span data-ttu-id="2db66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2db66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2db66-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2db66-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2db66-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db66-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2db66-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2db66-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2db66-108">Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="2db66-108">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2db66-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2db66-109">Prerequisites</span></span>
<span data-ttu-id="2db66-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db66-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2db66-112">Permission type</span></span>|<span data-ttu-id="2db66-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2db66-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2db66-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2db66-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2db66-115">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2db66-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2db66-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2db66-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2db66-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2db66-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2db66-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db66-118">Not supported.</span></span>|
|<span data-ttu-id="2db66-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2db66-119">Application</span></span>||
| <span data-ttu-id="2db66-120">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2db66-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2db66-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2db66-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="2db66-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2db66-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="2db66-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2db66-123">Request headers</span></span>
|<span data-ttu-id="2db66-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2db66-124">Header</span></span>|<span data-ttu-id="2db66-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2db66-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2db66-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2db66-126">Authorization</span></span>|<span data-ttu-id="2db66-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2db66-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2db66-128">Accept</span><span class="sxs-lookup"><span data-stu-id="2db66-128">Accept</span></span>|<span data-ttu-id="2db66-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2db66-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2db66-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2db66-130">Request body</span></span>
<span data-ttu-id="2db66-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2db66-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2db66-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2db66-132">Response</span></span>
<span data-ttu-id="2db66-133">В случае успеха эта функция возвращает код `200 OK` отклика и объект **девицеандаппманажементассигнедролеид** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2db66-133">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2db66-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2db66-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="2db66-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2db66-135">Request</span></span>
<span data-ttu-id="2db66-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2db66-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="2db66-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2db66-137">Response</span></span>
<span data-ttu-id="2db66-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2db66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











