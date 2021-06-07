---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83d642101b73ddb82765e8c2ec51d7205a48f3ab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752576"
---
# <a name="assign-action"></a><span data-ttu-id="b5572-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="b5572-103">assign action</span></span>

<span data-ttu-id="b5572-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5572-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5572-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b5572-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5572-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b5572-107">Prerequisites</span></span>
<span data-ttu-id="b5572-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5572-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5572-110">Permission type</span></span>|<span data-ttu-id="b5572-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5572-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5572-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5572-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5572-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5572-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5572-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5572-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5572-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5572-115">Not supported.</span></span>|
|<span data-ttu-id="b5572-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5572-116">Application</span></span>|<span data-ttu-id="b5572-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5572-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5572-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5572-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b5572-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5572-119">Request headers</span></span>
|<span data-ttu-id="b5572-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5572-120">Header</span></span>|<span data-ttu-id="b5572-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5572-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5572-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5572-122">Authorization</span></span>|<span data-ttu-id="b5572-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5572-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5572-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5572-124">Accept</span></span>|<span data-ttu-id="b5572-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5572-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5572-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5572-126">Request body</span></span>
<span data-ttu-id="b5572-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5572-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b5572-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b5572-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b5572-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5572-129">Property</span></span>|<span data-ttu-id="b5572-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5572-130">Type</span></span>|<span data-ttu-id="b5572-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5572-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5572-132">assignments</span><span class="sxs-lookup"><span data-stu-id="b5572-132">assignments</span></span>|<span data-ttu-id="b5572-133">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5572-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="b5572-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b5572-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b5572-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5572-135">Response</span></span>
<span data-ttu-id="b5572-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b5572-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b5572-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b5572-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5572-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5572-138">Request</span></span>
<span data-ttu-id="b5572-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5572-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 338

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b5572-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5572-140">Response</span></span>
<span data-ttu-id="b5572-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5572-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




