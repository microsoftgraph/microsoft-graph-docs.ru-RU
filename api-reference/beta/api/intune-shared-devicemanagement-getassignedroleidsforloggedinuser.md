---
title: функция getAssignedRoleIdsForLoggedInUser
description: Извлекает назначенное определение роли и назначения ролей для пользователя, который в настоящее время проходит проверку подлинности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3b0a8e4755ba6361bcb8d92dae4fe6c2e66eb65
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159460"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="68a5c-103">функция getAssignedRoleIdsForLoggedInUser</span><span class="sxs-lookup"><span data-stu-id="68a5c-103">getAssignedRoleIdsForLoggedInUser function</span></span>

<span data-ttu-id="68a5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68a5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68a5c-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="68a5c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68a5c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68a5c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68a5c-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68a5c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68a5c-108">Извлекает назначенное определение роли и назначения ролей для пользователя, который в настоящее время проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="68a5c-108">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68a5c-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68a5c-109">Prerequisites</span></span>
<span data-ttu-id="68a5c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a5c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68a5c-112">Permission type</span></span>|<span data-ttu-id="68a5c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68a5c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68a5c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68a5c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="68a5c-115">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="68a5c-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="68a5c-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="68a5c-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="68a5c-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68a5c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68a5c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68a5c-118">Not supported.</span></span>|
|<span data-ttu-id="68a5c-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="68a5c-119">Application</span></span>||
| <span data-ttu-id="68a5c-120">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="68a5c-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="68a5c-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="68a5c-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="68a5c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68a5c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="68a5c-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68a5c-123">Request headers</span></span>
|<span data-ttu-id="68a5c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68a5c-124">Header</span></span>|<span data-ttu-id="68a5c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="68a5c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68a5c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="68a5c-126">Authorization</span></span>|<span data-ttu-id="68a5c-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68a5c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68a5c-128">Accept</span><span class="sxs-lookup"><span data-stu-id="68a5c-128">Accept</span></span>|<span data-ttu-id="68a5c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="68a5c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a5c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68a5c-130">Request body</span></span>
<span data-ttu-id="68a5c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68a5c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68a5c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="68a5c-132">Response</span></span>
<span data-ttu-id="68a5c-133">В случае успешного выполнения эта функция возвращает код ответа и `200 OK` **устройствоAndAppManagementAssignedRoleId** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68a5c-133">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a5c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="68a5c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="68a5c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="68a5c-135">Request</span></span>
<span data-ttu-id="68a5c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68a5c-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="68a5c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="68a5c-137">Response</span></span>
<span data-ttu-id="68a5c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68a5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












