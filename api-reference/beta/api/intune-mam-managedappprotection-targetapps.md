---
title: Действие targetApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cf2db211b37993cb68ae40f5024f0c77110b96a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157920"
---
# <a name="targetapps-action"></a><span data-ttu-id="eeb98-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="eeb98-103">targetApps action</span></span>

<span data-ttu-id="eeb98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeb98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeb98-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeb98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeb98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeb98-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eeb98-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeb98-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eeb98-108">Prerequisites</span></span>
<span data-ttu-id="eeb98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb98-111">Permission type</span></span>|<span data-ttu-id="eeb98-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeb98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeb98-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeb98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eeb98-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeb98-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eeb98-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeb98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeb98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb98-116">Not supported.</span></span>|
|<span data-ttu-id="eeb98-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeb98-117">Application</span></span>|<span data-ttu-id="eeb98-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeb98-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeb98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeb98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="eeb98-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eeb98-120">Request headers</span></span>
|<span data-ttu-id="eeb98-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eeb98-121">Header</span></span>|<span data-ttu-id="eeb98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eeb98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeb98-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeb98-123">Authorization</span></span>|<span data-ttu-id="eeb98-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeb98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeb98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eeb98-125">Accept</span></span>|<span data-ttu-id="eeb98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eeb98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeb98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeb98-127">Request body</span></span>
<span data-ttu-id="eeb98-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeb98-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eeb98-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="eeb98-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eeb98-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeb98-130">Property</span></span>|<span data-ttu-id="eeb98-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eeb98-131">Type</span></span>|<span data-ttu-id="eeb98-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeb98-133">apps</span><span class="sxs-lookup"><span data-stu-id="eeb98-133">apps</span></span>|<span data-ttu-id="eeb98-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eeb98-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="eeb98-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="eeb98-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eeb98-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="eeb98-136">Response</span></span>
<span data-ttu-id="eeb98-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eeb98-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eeb98-138">Пример</span><span class="sxs-lookup"><span data-stu-id="eeb98-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeb98-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeb98-139">Request</span></span>
<span data-ttu-id="eeb98-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeb98-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 336

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="eeb98-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeb98-141">Response</span></span>
<span data-ttu-id="eeb98-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eeb98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




