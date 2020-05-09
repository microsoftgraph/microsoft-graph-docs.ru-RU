---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1a91a55427f7c59aa912148e62aad23edb26a0a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177536"
---
# <a name="assign-action"></a><span data-ttu-id="4fa4d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="4fa4d-103">assign action</span></span>

<span data-ttu-id="4fa4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fa4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fa4d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fa4d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fa4d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fa4d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4fa4d-108">Prerequisites</span></span>
<span data-ttu-id="4fa4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fa4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fa4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa4d-111">Permission type</span></span>|<span data-ttu-id="4fa4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fa4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fa4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fa4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fa4d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fa4d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4fa4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fa4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fa4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-116">Not supported.</span></span>|
|<span data-ttu-id="4fa4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fa4d-117">Application</span></span>|<span data-ttu-id="4fa4d-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fa4d-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fa4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fa4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/{roleScopeTagId}/assign
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4fa4d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4fa4d-120">Request headers</span></span>
|<span data-ttu-id="4fa4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fa4d-121">Header</span></span>|<span data-ttu-id="4fa4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fa4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fa4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fa4d-123">Authorization</span></span>|<span data-ttu-id="4fa4d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fa4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fa4d-125">Accept</span></span>|<span data-ttu-id="4fa4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fa4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fa4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fa4d-127">Request body</span></span>
<span data-ttu-id="4fa4d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4fa4d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4fa4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fa4d-130">Property</span></span>|<span data-ttu-id="4fa4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fa4d-131">Type</span></span>|<span data-ttu-id="4fa4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fa4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa4d-133">assignments</span><span class="sxs-lookup"><span data-stu-id="4fa4d-133">assignments</span></span>|<span data-ttu-id="4fa4d-134">Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4fa4d-134">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="4fa4d-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4fa4d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4fa4d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fa4d-136">Response</span></span>
<span data-ttu-id="4fa4d-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-137">If successful, this action returns a `200 OK` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fa4d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4fa4d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fa4d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fa4d-139">Request</span></span>
<span data-ttu-id="4fa4d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}/assign

Content-type: application/json
Content-length: 262

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4fa4d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fa4d-141">Response</span></span>
<span data-ttu-id="4fa4d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fa4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



