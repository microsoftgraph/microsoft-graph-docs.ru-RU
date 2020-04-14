---
title: Действие targetApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef9b9b9f480ad62cef2c195d17d464af3418897b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444544"
---
# <a name="targetapps-action"></a><span data-ttu-id="a59a7-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="a59a7-103">targetApps action</span></span>

<span data-ttu-id="a59a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a59a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a59a7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a59a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a59a7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a59a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a59a7-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a59a7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a59a7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a59a7-108">Prerequisites</span></span>
<span data-ttu-id="a59a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a59a7-111">Permission type</span></span>|<span data-ttu-id="a59a7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a59a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a59a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a59a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a59a7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59a7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a59a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a59a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a59a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a59a7-116">Not supported.</span></span>|
|<span data-ttu-id="a59a7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a59a7-117">Application</span></span>|<span data-ttu-id="a59a7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59a7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a59a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a59a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="a59a7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a59a7-120">Request headers</span></span>
|<span data-ttu-id="a59a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a59a7-121">Header</span></span>|<span data-ttu-id="a59a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a59a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a59a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a59a7-123">Authorization</span></span>|<span data-ttu-id="a59a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a59a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a59a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a59a7-125">Accept</span></span>|<span data-ttu-id="a59a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a59a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a59a7-127">Request body</span></span>
<span data-ttu-id="a59a7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a59a7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a59a7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a59a7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a59a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a59a7-130">Property</span></span>|<span data-ttu-id="a59a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a59a7-131">Type</span></span>|<span data-ttu-id="a59a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a59a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59a7-133">apps</span><span class="sxs-lookup"><span data-stu-id="a59a7-133">apps</span></span>|<span data-ttu-id="a59a7-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a59a7-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="a59a7-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a59a7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a59a7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a59a7-136">Response</span></span>
<span data-ttu-id="a59a7-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a59a7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a59a7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a59a7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a59a7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a59a7-139">Request</span></span>
<span data-ttu-id="a59a7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a59a7-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a59a7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a59a7-141">Response</span></span>
<span data-ttu-id="a59a7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a59a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



