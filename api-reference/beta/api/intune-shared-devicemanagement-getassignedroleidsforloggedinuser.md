---
title: Функция Жетассигнедролеидсфорлогжединусер
description: Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 095b07f76d6202d1ec493a187f61e141ca3813c3
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086069"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="e08b2-103">Функция Жетассигнедролеидсфорлогжединусер</span><span class="sxs-lookup"><span data-stu-id="e08b2-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="e08b2-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e08b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e08b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e08b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e08b2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e08b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e08b2-107">Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="e08b2-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e08b2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e08b2-108">Prerequisites</span></span>
<span data-ttu-id="e08b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e08b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e08b2-111">Permission type</span></span>|<span data-ttu-id="e08b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e08b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e08b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e08b2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e08b2-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="e08b2-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="e08b2-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e08b2-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e08b2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e08b2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e08b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e08b2-117">Not supported.</span></span>|
|<span data-ttu-id="e08b2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e08b2-118">Application</span></span>||
| <span data-ttu-id="e08b2-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="e08b2-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="e08b2-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e08b2-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="e08b2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e08b2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="e08b2-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e08b2-122">Request headers</span></span>
|<span data-ttu-id="e08b2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e08b2-123">Header</span></span>|<span data-ttu-id="e08b2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e08b2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e08b2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e08b2-125">Authorization</span></span>|<span data-ttu-id="e08b2-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e08b2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e08b2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e08b2-127">Accept</span></span>|<span data-ttu-id="e08b2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e08b2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e08b2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e08b2-129">Request body</span></span>
<span data-ttu-id="e08b2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e08b2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e08b2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e08b2-131">Response</span></span>
<span data-ttu-id="e08b2-132">В случае успеха эта функция возвращает код `200 OK` отклика и объект **девицеандаппманажементассигнедролеид** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e08b2-132">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e08b2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e08b2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e08b2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e08b2-134">Request</span></span>
<span data-ttu-id="e08b2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e08b2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="e08b2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e08b2-136">Response</span></span>
<span data-ttu-id="e08b2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e08b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














