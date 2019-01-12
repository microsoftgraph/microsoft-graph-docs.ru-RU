---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50e87574a14bea80bb154b4cb981ff9a8d9cd56b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964881"
---
# <a name="assign-action"></a><span data-ttu-id="9c131-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="9c131-103">assign action</span></span>

> <span data-ttu-id="9c131-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c131-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c131-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c131-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c131-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9c131-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c131-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9c131-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c131-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9c131-108">Prerequisites</span></span>
<span data-ttu-id="9c131-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c131-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c131-111">Permission type</span></span>|<span data-ttu-id="9c131-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c131-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c131-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c131-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c131-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c131-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c131-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c131-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c131-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c131-116">Not supported.</span></span>|
|<span data-ttu-id="9c131-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c131-117">Application</span></span>|<span data-ttu-id="9c131-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c131-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c131-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c131-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9c131-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c131-120">Request headers</span></span>
|<span data-ttu-id="9c131-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c131-121">Header</span></span>|<span data-ttu-id="9c131-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c131-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c131-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c131-123">Authorization</span></span>|<span data-ttu-id="9c131-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9c131-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c131-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c131-125">Accept</span></span>|<span data-ttu-id="9c131-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c131-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c131-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c131-127">Request body</span></span>
<span data-ttu-id="9c131-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c131-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9c131-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9c131-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9c131-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c131-130">Property</span></span>|<span data-ttu-id="9c131-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9c131-131">Type</span></span>|<span data-ttu-id="9c131-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9c131-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c131-133">assignments</span><span class="sxs-lookup"><span data-stu-id="9c131-133">assignments</span></span>|<span data-ttu-id="9c131-134">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9c131-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9c131-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9c131-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c131-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c131-136">Response</span></span>
<span data-ttu-id="9c131-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c131-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c131-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9c131-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c131-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c131-139">Request</span></span>
<span data-ttu-id="9c131-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c131-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c131-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c131-141">Response</span></span>
<span data-ttu-id="9c131-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c131-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





