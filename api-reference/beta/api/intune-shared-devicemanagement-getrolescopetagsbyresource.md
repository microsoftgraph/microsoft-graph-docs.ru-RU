---
title: функция getRoleScopeTagsByResource
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47742e8ea1611810bf36be8ca3c004c17b07425b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865945"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="6f92c-103">функция getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="6f92c-103">getRoleScopeTagsByResource function</span></span>

<span data-ttu-id="6f92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f92c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f92c-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="6f92c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f92c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f92c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f92c-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f92c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f92c-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f92c-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f92c-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f92c-109">Prerequisites</span></span>
<span data-ttu-id="6f92c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f92c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f92c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f92c-112">Permission type</span></span>|<span data-ttu-id="6f92c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f92c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f92c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f92c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f92c-115">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6f92c-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6f92c-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f92c-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6f92c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f92c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f92c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f92c-118">Not supported.</span></span>|
|<span data-ttu-id="6f92c-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6f92c-119">Application</span></span>||
| <span data-ttu-id="6f92c-120">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="6f92c-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="6f92c-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f92c-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f92c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f92c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="6f92c-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f92c-123">Request headers</span></span>
|<span data-ttu-id="6f92c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f92c-124">Header</span></span>|<span data-ttu-id="6f92c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6f92c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f92c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f92c-126">Authorization</span></span>|<span data-ttu-id="6f92c-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f92c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f92c-128">Accept</span><span class="sxs-lookup"><span data-stu-id="6f92c-128">Accept</span></span>|<span data-ttu-id="6f92c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6f92c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f92c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f92c-130">Request body</span></span>
<span data-ttu-id="6f92c-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6f92c-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f92c-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6f92c-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f92c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f92c-133">Property</span></span>|<span data-ttu-id="6f92c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6f92c-134">Type</span></span>|<span data-ttu-id="6f92c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6f92c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f92c-136">resource</span><span class="sxs-lookup"><span data-stu-id="6f92c-136">resource</span></span>|<span data-ttu-id="6f92c-137">String</span><span class="sxs-lookup"><span data-stu-id="6f92c-137">String</span></span>|<span data-ttu-id="6f92c-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f92c-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f92c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f92c-139">Response</span></span>
<span data-ttu-id="6f92c-140">В случае успешной работы эта функция возвращает код отклика и коллекцию `200 OK` [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6f92c-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f92c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6f92c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f92c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f92c-142">Request</span></span>
<span data-ttu-id="6f92c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f92c-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6f92c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f92c-144">Response</span></span>
<span data-ttu-id="6f92c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f92c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```










