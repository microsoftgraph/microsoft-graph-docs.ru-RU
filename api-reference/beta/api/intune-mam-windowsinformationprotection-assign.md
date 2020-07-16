---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94f2c18c3c9e0e50fa40b2d8e5a3243405a8de0f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791877"
---
# <a name="assign-action"></a><span data-ttu-id="127b0-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="127b0-103">assign action</span></span>

<span data-ttu-id="127b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="127b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="127b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="127b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="127b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127b0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="127b0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="127b0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="127b0-108">Prerequisites</span></span>
<span data-ttu-id="127b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="127b0-111">Permission type</span></span>|<span data-ttu-id="127b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="127b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="127b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="127b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="127b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="127b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="127b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="127b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="127b0-116">Not supported.</span></span>|
|<span data-ttu-id="127b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="127b0-117">Application</span></span>|<span data-ttu-id="127b0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127b0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="127b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="127b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="127b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="127b0-120">Request headers</span></span>
|<span data-ttu-id="127b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="127b0-121">Header</span></span>|<span data-ttu-id="127b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="127b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="127b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="127b0-123">Authorization</span></span>|<span data-ttu-id="127b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="127b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="127b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="127b0-125">Accept</span></span>|<span data-ttu-id="127b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="127b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="127b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="127b0-127">Request body</span></span>
<span data-ttu-id="127b0-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="127b0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="127b0-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="127b0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="127b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="127b0-130">Property</span></span>|<span data-ttu-id="127b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="127b0-131">Type</span></span>|<span data-ttu-id="127b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="127b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127b0-133">assignments</span><span class="sxs-lookup"><span data-stu-id="127b0-133">assignments</span></span>|<span data-ttu-id="127b0-134">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="127b0-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="127b0-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="127b0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="127b0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="127b0-136">Response</span></span>
<span data-ttu-id="127b0-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="127b0-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="127b0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="127b0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="127b0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="127b0-139">Request</span></span>
<span data-ttu-id="127b0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="127b0-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 514

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="127b0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="127b0-141">Response</span></span>
<span data-ttu-id="127b0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="127b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



