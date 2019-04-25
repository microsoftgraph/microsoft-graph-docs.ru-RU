---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13ef56b1e2cacb922e5cca9cb57e924062613eb9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529305"
---
# <a name="assign-action"></a><span data-ttu-id="5edd5-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="5edd5-103">assign action</span></span>

> <span data-ttu-id="5edd5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5edd5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5edd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5edd5-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5edd5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5edd5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5edd5-107">Prerequisites</span></span>
<span data-ttu-id="5edd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5edd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5edd5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5edd5-110">Permission type</span></span>|<span data-ttu-id="5edd5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5edd5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5edd5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5edd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5edd5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5edd5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5edd5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5edd5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5edd5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edd5-115">Not supported.</span></span>|
|<span data-ttu-id="5edd5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5edd5-116">Application</span></span>|<span data-ttu-id="5edd5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edd5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5edd5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5edd5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5edd5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5edd5-119">Request headers</span></span>
|<span data-ttu-id="5edd5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5edd5-120">Header</span></span>|<span data-ttu-id="5edd5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5edd5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5edd5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5edd5-122">Authorization</span></span>|<span data-ttu-id="5edd5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5edd5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5edd5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5edd5-124">Accept</span></span>|<span data-ttu-id="5edd5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5edd5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5edd5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5edd5-126">Request body</span></span>
<span data-ttu-id="5edd5-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5edd5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5edd5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5edd5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5edd5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5edd5-129">Property</span></span>|<span data-ttu-id="5edd5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5edd5-130">Type</span></span>|<span data-ttu-id="5edd5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5edd5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5edd5-132">assignments</span><span class="sxs-lookup"><span data-stu-id="5edd5-132">assignments</span></span>|<span data-ttu-id="5edd5-133">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5edd5-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="5edd5-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5edd5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5edd5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5edd5-135">Response</span></span>
<span data-ttu-id="5edd5-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5edd5-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5edd5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5edd5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5edd5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5edd5-138">Request</span></span>
<span data-ttu-id="5edd5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5edd5-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5edd5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5edd5-140">Response</span></span>
<span data-ttu-id="5edd5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5edd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





