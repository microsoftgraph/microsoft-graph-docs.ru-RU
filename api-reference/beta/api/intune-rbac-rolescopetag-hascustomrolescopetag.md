---
title: Функция Хаскустомролескопетаг
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00d3425a8f34b6d1cd09384f7ed7062d31da978b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801581"
---
# <a name="hascustomrolescopetag-function"></a><span data-ttu-id="79053-103">Функция Хаскустомролескопетаг</span><span class="sxs-lookup"><span data-stu-id="79053-103">hasCustomRoleScopeTag function</span></span>

> <span data-ttu-id="79053-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79053-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79053-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79053-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79053-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="79053-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79053-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79053-107">Prerequisites</span></span>
<span data-ttu-id="79053-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79053-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79053-110">Permission type</span></span>|<span data-ttu-id="79053-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79053-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79053-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79053-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79053-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="79053-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="79053-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79053-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79053-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79053-115">Not supported.</span></span>|
|<span data-ttu-id="79053-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="79053-116">Application</span></span>|<span data-ttu-id="79053-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="79053-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79053-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79053-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/hasCustomRoleScopeTag
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/hasCustomRoleScopeTag
```

## <a name="request-headers"></a><span data-ttu-id="79053-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="79053-119">Request headers</span></span>
|<span data-ttu-id="79053-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79053-120">Header</span></span>|<span data-ttu-id="79053-121">Значение</span><span class="sxs-lookup"><span data-stu-id="79053-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79053-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79053-122">Authorization</span></span>|<span data-ttu-id="79053-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79053-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79053-124">Accept</span><span class="sxs-lookup"><span data-stu-id="79053-124">Accept</span></span>|<span data-ttu-id="79053-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79053-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79053-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79053-126">Request body</span></span>
<span data-ttu-id="79053-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79053-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79053-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="79053-128">Response</span></span>
<span data-ttu-id="79053-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79053-129">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79053-130">Пример</span><span class="sxs-lookup"><span data-stu-id="79053-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79053-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79053-131">Request</span></span>
<span data-ttu-id="79053-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79053-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/hasCustomRoleScopeTag
```

### <a name="response"></a><span data-ttu-id="79053-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79053-133">Response</span></span>
<span data-ttu-id="79053-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79053-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




