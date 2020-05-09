---
title: Действие targetApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a65481a3aca705d8aa0b003fc47787ee81817daa
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178621"
---
# <a name="targetapps-action"></a><span data-ttu-id="92292-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="92292-103">targetApps action</span></span>

<span data-ttu-id="92292-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92292-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92292-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92292-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92292-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92292-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92292-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="92292-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92292-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="92292-108">Prerequisites</span></span>
<span data-ttu-id="92292-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92292-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92292-111">Permission type</span></span>|<span data-ttu-id="92292-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92292-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92292-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92292-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92292-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92292-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92292-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92292-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92292-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92292-116">Not supported.</span></span>|
|<span data-ttu-id="92292-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92292-117">Application</span></span>|<span data-ttu-id="92292-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92292-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92292-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92292-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="92292-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92292-120">Request headers</span></span>
|<span data-ttu-id="92292-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92292-121">Header</span></span>|<span data-ttu-id="92292-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92292-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92292-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92292-123">Authorization</span></span>|<span data-ttu-id="92292-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92292-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92292-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92292-125">Accept</span></span>|<span data-ttu-id="92292-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92292-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92292-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92292-127">Request body</span></span>
<span data-ttu-id="92292-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92292-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92292-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="92292-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92292-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92292-130">Property</span></span>|<span data-ttu-id="92292-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92292-131">Type</span></span>|<span data-ttu-id="92292-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92292-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92292-133">apps</span><span class="sxs-lookup"><span data-stu-id="92292-133">apps</span></span>|<span data-ttu-id="92292-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92292-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="92292-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="92292-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92292-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="92292-136">Response</span></span>
<span data-ttu-id="92292-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92292-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92292-138">Пример</span><span class="sxs-lookup"><span data-stu-id="92292-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="92292-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="92292-139">Request</span></span>
<span data-ttu-id="92292-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92292-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 335

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="92292-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="92292-141">Response</span></span>
<span data-ttu-id="92292-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



