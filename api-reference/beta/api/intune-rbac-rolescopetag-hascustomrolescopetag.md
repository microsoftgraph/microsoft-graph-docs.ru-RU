---
title: Функция Хаскустомролескопетаг
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a34f986559f7ba81465f51b0858577ee92a5c6da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437611"
---
# <a name="hascustomrolescopetag-function"></a><span data-ttu-id="3c9e4-103">Функция Хаскустомролескопетаг</span><span class="sxs-lookup"><span data-stu-id="3c9e4-103">hasCustomRoleScopeTag function</span></span>

<span data-ttu-id="3c9e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c9e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c9e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c9e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c9e4-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c9e4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c9e4-108">Prerequisites</span></span>
<span data-ttu-id="3c9e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c9e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c9e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c9e4-111">Permission type</span></span>|<span data-ttu-id="3c9e4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c9e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c9e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c9e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c9e4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c9e4-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3c9e4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c9e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c9e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-116">Not supported.</span></span>|
|<span data-ttu-id="3c9e4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c9e4-117">Application</span></span>|<span data-ttu-id="3c9e4-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c9e4-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c9e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c9e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/hasCustomRoleScopeTag
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/hasCustomRoleScopeTag
```

## <a name="request-headers"></a><span data-ttu-id="3c9e4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3c9e4-120">Request headers</span></span>
|<span data-ttu-id="3c9e4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c9e4-121">Header</span></span>|<span data-ttu-id="3c9e4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c9e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c9e4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c9e4-123">Authorization</span></span>|<span data-ttu-id="3c9e4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c9e4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c9e4-125">Accept</span></span>|<span data-ttu-id="3c9e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c9e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c9e4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c9e4-127">Request body</span></span>
<span data-ttu-id="3c9e4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c9e4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c9e4-129">Response</span></span>
<span data-ttu-id="3c9e4-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9e4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3c9e4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c9e4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c9e4-132">Request</span></span>
<span data-ttu-id="3c9e4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/hasCustomRoleScopeTag
```

### <a name="response"></a><span data-ttu-id="3c9e4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c9e4-134">Response</span></span>
<span data-ttu-id="3c9e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c9e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



