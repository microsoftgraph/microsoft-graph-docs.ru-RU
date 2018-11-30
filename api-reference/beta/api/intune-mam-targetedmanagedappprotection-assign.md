---
title: Действие assign
description: Н/Д
ms.openlocfilehash: d2ca94973c66486fc8cc9aeb3c4c793471ff2e13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082190"
---
# <a name="assign-action"></a><span data-ttu-id="9b839-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="9b839-103">assign action</span></span>

> <span data-ttu-id="9b839-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b839-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b839-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b839-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b839-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9b839-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b839-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9b839-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b839-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9b839-108">Prerequisites</span></span>
<span data-ttu-id="9b839-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b839-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b839-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b839-111">Permission type</span></span>|<span data-ttu-id="9b839-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b839-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b839-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b839-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b839-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b839-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b839-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b839-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b839-116">Not supported.</span></span>|
|<span data-ttu-id="9b839-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b839-117">Application</span></span>|<span data-ttu-id="9b839-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b839-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b839-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b839-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9b839-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b839-120">Request headers</span></span>
|<span data-ttu-id="9b839-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b839-121">Header</span></span>|<span data-ttu-id="9b839-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b839-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b839-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b839-123">Authorization</span></span>|<span data-ttu-id="9b839-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9b839-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b839-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b839-125">Accept</span></span>|<span data-ttu-id="9b839-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b839-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b839-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b839-127">Request body</span></span>
<span data-ttu-id="9b839-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b839-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9b839-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9b839-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9b839-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b839-130">Property</span></span>|<span data-ttu-id="9b839-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b839-131">Type</span></span>|<span data-ttu-id="9b839-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b839-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b839-133">assignments</span><span class="sxs-lookup"><span data-stu-id="9b839-133">assignments</span></span>|<span data-ttu-id="9b839-134">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b839-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9b839-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9b839-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b839-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b839-136">Response</span></span>
<span data-ttu-id="9b839-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b839-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9b839-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9b839-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b839-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b839-139">Request</span></span>
<span data-ttu-id="9b839-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b839-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="9b839-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b839-141">Response</span></span>
<span data-ttu-id="9b839-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9b839-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





