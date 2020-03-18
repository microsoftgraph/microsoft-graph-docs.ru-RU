---
title: Функция Жетассигнедролеидсфорлогжединусер
description: Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b80d34792b54fe6b5f041773179abfea79a0f2f0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801070"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="aef7a-103">Функция Жетассигнедролеидсфорлогжединусер</span><span class="sxs-lookup"><span data-stu-id="aef7a-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="aef7a-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aef7a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aef7a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aef7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aef7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef7a-107">Извлекает назначенные определения ролей и назначения ролей для текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="aef7a-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aef7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aef7a-108">Prerequisites</span></span>
<span data-ttu-id="aef7a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aef7a-111">Permission type</span></span>|<span data-ttu-id="aef7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aef7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aef7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aef7a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aef7a-114">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="aef7a-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="aef7a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef7a-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="aef7a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aef7a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aef7a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef7a-117">Not supported.</span></span>|
|<span data-ttu-id="aef7a-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="aef7a-118">Application</span></span>||
| <span data-ttu-id="aef7a-119">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="aef7a-119">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="aef7a-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef7a-120">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="aef7a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aef7a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="aef7a-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aef7a-122">Request headers</span></span>
|<span data-ttu-id="aef7a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aef7a-123">Header</span></span>|<span data-ttu-id="aef7a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="aef7a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aef7a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aef7a-125">Authorization</span></span>|<span data-ttu-id="aef7a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef7a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aef7a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="aef7a-127">Accept</span></span>|<span data-ttu-id="aef7a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aef7a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef7a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aef7a-129">Request body</span></span>
<span data-ttu-id="aef7a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aef7a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aef7a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="aef7a-131">Response</span></span>
<span data-ttu-id="aef7a-132">В случае успеха эта функция возвращает код `200 OK` отклика и объект **девицеандаппманажементассигнедролеид** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aef7a-132">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef7a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aef7a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="aef7a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef7a-134">Request</span></span>
<span data-ttu-id="aef7a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aef7a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="aef7a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef7a-136">Response</span></span>
<span data-ttu-id="aef7a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aef7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












