---
title: Действие targetApps
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95ccefee7631e79a4184ece916126d150ef8af21
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903532"
---
# <a name="targetapps-action"></a><span data-ttu-id="422c4-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="422c4-103">targetApps action</span></span>

> <span data-ttu-id="422c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="422c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="422c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="422c4-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="422c4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="422c4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="422c4-107">Prerequisites</span></span>
<span data-ttu-id="422c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="422c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422c4-110">Permission type</span></span>|<span data-ttu-id="422c4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="422c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="422c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="422c4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422c4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="422c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="422c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-115">Not supported.</span></span>|
|<span data-ttu-id="422c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="422c4-116">Application</span></span>|<span data-ttu-id="422c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="422c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="422c4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="422c4-119">Request headers</span></span>
|<span data-ttu-id="422c4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="422c4-120">Header</span></span>|<span data-ttu-id="422c4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="422c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="422c4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="422c4-122">Authorization</span></span>|<span data-ttu-id="422c4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="422c4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="422c4-124">Accept</span></span>|<span data-ttu-id="422c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="422c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="422c4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="422c4-126">Request body</span></span>
<span data-ttu-id="422c4-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="422c4-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="422c4-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="422c4-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="422c4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="422c4-129">Property</span></span>|<span data-ttu-id="422c4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="422c4-130">Type</span></span>|<span data-ttu-id="422c4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="422c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="422c4-132">apps</span><span class="sxs-lookup"><span data-stu-id="422c4-132">apps</span></span>|<span data-ttu-id="422c4-133">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="422c4-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="422c4-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="422c4-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="422c4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="422c4-135">Response</span></span>
<span data-ttu-id="422c4-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="422c4-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="422c4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="422c4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="422c4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="422c4-138">Request</span></span>
<span data-ttu-id="422c4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422c4-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="422c4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="422c4-140">Response</span></span>
<span data-ttu-id="422c4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="422c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




