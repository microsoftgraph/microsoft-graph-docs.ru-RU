---
title: Действие assign
description: Н/Д
ms.openlocfilehash: 928067d1058df303c6963d54d4322c2b41ddddb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024364"
---
# <a name="assign-action"></a><span data-ttu-id="833f6-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="833f6-103">assign action</span></span>

> <span data-ttu-id="833f6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="833f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="833f6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="833f6-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="833f6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="833f6-106">Prerequisites</span></span>
<span data-ttu-id="833f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="833f6-109">Permission type</span></span>|<span data-ttu-id="833f6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="833f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="833f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="833f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="833f6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833f6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="833f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="833f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="833f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833f6-114">Not supported.</span></span>|
|<span data-ttu-id="833f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="833f6-115">Application</span></span>|<span data-ttu-id="833f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="833f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="833f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="833f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="833f6-118">Request headers</span></span>
|<span data-ttu-id="833f6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="833f6-119">Header</span></span>|<span data-ttu-id="833f6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="833f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="833f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="833f6-121">Authorization</span></span>|<span data-ttu-id="833f6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="833f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="833f6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="833f6-123">Accept</span></span>|<span data-ttu-id="833f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="833f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="833f6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="833f6-125">Request body</span></span>
<span data-ttu-id="833f6-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="833f6-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="833f6-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="833f6-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="833f6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="833f6-128">Property</span></span>|<span data-ttu-id="833f6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="833f6-129">Type</span></span>|<span data-ttu-id="833f6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="833f6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="833f6-131">assignments</span><span class="sxs-lookup"><span data-stu-id="833f6-131">assignments</span></span>|<span data-ttu-id="833f6-132">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="833f6-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="833f6-133">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="833f6-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="833f6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="833f6-134">Response</span></span>
<span data-ttu-id="833f6-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="833f6-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="833f6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="833f6-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="833f6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="833f6-137">Request</span></span>
<span data-ttu-id="833f6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="833f6-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="833f6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="833f6-139">Response</span></span>
<span data-ttu-id="833f6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="833f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



