---
title: Действие assign
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 70d66bfda498c6fbfa7065e0d35006563567bb08
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359075"
---
# <a name="assign-action"></a><span data-ttu-id="e992d-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e992d-103">assign action</span></span>

> <span data-ttu-id="e992d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e992d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e992d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e992d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e992d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e992d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e992d-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e992d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e992d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e992d-108">Prerequisites</span></span>
<span data-ttu-id="e992d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e992d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e992d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e992d-111">Permission type</span></span>|<span data-ttu-id="e992d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e992d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e992d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e992d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e992d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e992d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e992d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e992d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e992d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e992d-116">Not supported.</span></span>|
|<span data-ttu-id="e992d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e992d-117">Application</span></span>|<span data-ttu-id="e992d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e992d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e992d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e992d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e992d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e992d-120">Request headers</span></span>
|<span data-ttu-id="e992d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e992d-121">Header</span></span>|<span data-ttu-id="e992d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e992d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e992d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e992d-123">Authorization</span></span>|<span data-ttu-id="e992d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e992d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e992d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e992d-125">Accept</span></span>|<span data-ttu-id="e992d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e992d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e992d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e992d-127">Request body</span></span>
<span data-ttu-id="e992d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e992d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e992d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e992d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e992d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e992d-130">Property</span></span>|<span data-ttu-id="e992d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e992d-131">Type</span></span>|<span data-ttu-id="e992d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e992d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e992d-133">assignments</span><span class="sxs-lookup"><span data-stu-id="e992d-133">assignments</span></span>|<span data-ttu-id="e992d-134">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e992d-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e992d-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e992d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e992d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e992d-136">Response</span></span>
<span data-ttu-id="e992d-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e992d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e992d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e992d-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e992d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e992d-139">Request</span></span>
<span data-ttu-id="e992d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e992d-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e992d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e992d-141">Response</span></span>
<span data-ttu-id="e992d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e992d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





