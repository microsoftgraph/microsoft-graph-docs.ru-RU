---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2f0c739ac81be301b3f283b288ff055d69752ff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397717"
---
# <a name="assign-action"></a><span data-ttu-id="e7d16-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e7d16-103">assign action</span></span>

<span data-ttu-id="e7d16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7d16-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7d16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d16-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e7d16-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7d16-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7d16-107">Prerequisites</span></span>
<span data-ttu-id="e7d16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7d16-110">Permission type</span></span>|<span data-ttu-id="e7d16-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7d16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7d16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d16-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d16-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7d16-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7d16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d16-115">Not supported.</span></span>|
|<span data-ttu-id="e7d16-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7d16-116">Application</span></span>|<span data-ttu-id="e7d16-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d16-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7d16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e7d16-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e7d16-119">Request headers</span></span>
|<span data-ttu-id="e7d16-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7d16-120">Header</span></span>|<span data-ttu-id="e7d16-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7d16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7d16-122">Authorization</span></span>|<span data-ttu-id="e7d16-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7d16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d16-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7d16-124">Accept</span></span>|<span data-ttu-id="e7d16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d16-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7d16-126">Request body</span></span>
<span data-ttu-id="e7d16-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7d16-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e7d16-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e7d16-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e7d16-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7d16-129">Property</span></span>|<span data-ttu-id="e7d16-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7d16-130">Type</span></span>|<span data-ttu-id="e7d16-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d16-132">assignments</span><span class="sxs-lookup"><span data-stu-id="e7d16-132">assignments</span></span>|<span data-ttu-id="e7d16-133">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e7d16-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e7d16-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7d16-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7d16-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7d16-135">Response</span></span>
<span data-ttu-id="e7d16-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7d16-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7d16-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e7d16-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7d16-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7d16-138">Request</span></span>
<span data-ttu-id="e7d16-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7d16-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e7d16-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7d16-140">Response</span></span>
<span data-ttu-id="e7d16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7d16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






