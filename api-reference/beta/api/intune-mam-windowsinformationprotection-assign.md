---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e527c17a53b3b8a11c97e790faaf78ee2d71fc0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153867"
---
# <a name="assign-action"></a><span data-ttu-id="92590-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="92590-103">assign action</span></span>

<span data-ttu-id="92590-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92590-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92590-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92590-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92590-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92590-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92590-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="92590-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92590-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="92590-108">Prerequisites</span></span>
<span data-ttu-id="92590-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92590-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92590-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92590-111">Permission type</span></span>|<span data-ttu-id="92590-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92590-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92590-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92590-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92590-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92590-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92590-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92590-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92590-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92590-116">Not supported.</span></span>|
|<span data-ttu-id="92590-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92590-117">Application</span></span>|<span data-ttu-id="92590-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92590-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92590-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92590-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="92590-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92590-120">Request headers</span></span>
|<span data-ttu-id="92590-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92590-121">Header</span></span>|<span data-ttu-id="92590-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92590-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92590-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92590-123">Authorization</span></span>|<span data-ttu-id="92590-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92590-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92590-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92590-125">Accept</span></span>|<span data-ttu-id="92590-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92590-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92590-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92590-127">Request body</span></span>
<span data-ttu-id="92590-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92590-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92590-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="92590-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92590-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92590-130">Property</span></span>|<span data-ttu-id="92590-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92590-131">Type</span></span>|<span data-ttu-id="92590-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92590-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92590-133">assignments</span><span class="sxs-lookup"><span data-stu-id="92590-133">assignments</span></span>|<span data-ttu-id="92590-134">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92590-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="92590-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="92590-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92590-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="92590-136">Response</span></span>
<span data-ttu-id="92590-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92590-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92590-138">Пример</span><span class="sxs-lookup"><span data-stu-id="92590-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="92590-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="92590-139">Request</span></span>
<span data-ttu-id="92590-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92590-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 582

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="92590-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="92590-141">Response</span></span>
<span data-ttu-id="92590-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92590-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




