---
title: функция getAssignedRoleDetails
description: Извлекает назначенное определение роли и назначения ролей для пользователя, который в настоящее время проходит проверку подлинности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e50ae596bd18d4d20b09da87018539c4ba598602
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148493"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="069ff-103">функция getAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="069ff-103">getAssignedRoleDetails function</span></span>

<span data-ttu-id="069ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="069ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="069ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="069ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="069ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="069ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="069ff-107">Извлекает назначенное определение роли и назначения ролей для пользователя, который в настоящее время проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="069ff-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="069ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="069ff-108">Prerequisites</span></span>
<span data-ttu-id="069ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="069ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="069ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="069ff-111">Permission type</span></span>|<span data-ttu-id="069ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="069ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="069ff-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="069ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="069ff-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069ff-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="069ff-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="069ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="069ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="069ff-116">Not supported.</span></span>|
|<span data-ttu-id="069ff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="069ff-117">Application</span></span>|<span data-ttu-id="069ff-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069ff-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="069ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="069ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="069ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="069ff-120">Request headers</span></span>
|<span data-ttu-id="069ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="069ff-121">Header</span></span>|<span data-ttu-id="069ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="069ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="069ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="069ff-123">Authorization</span></span>|<span data-ttu-id="069ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="069ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="069ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="069ff-125">Accept</span></span>|<span data-ttu-id="069ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="069ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="069ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="069ff-127">Request body</span></span>
<span data-ttu-id="069ff-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="069ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="069ff-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="069ff-129">Response</span></span>
<span data-ttu-id="069ff-130">В случае успешного выполнения эта функция возвращает код ответа и `200 OK` [устройствоAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="069ff-130">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="069ff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="069ff-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="069ff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="069ff-132">Request</span></span>
<span data-ttu-id="069ff-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="069ff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="069ff-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="069ff-134">Response</span></span>
<span data-ttu-id="069ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="069ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
    "roleDefinitionIds": [
      "Role Definition Ids value"
    ],
    "roleAssignmentIds": [
      "Role Assignment Ids value"
    ]
  }
}
```




