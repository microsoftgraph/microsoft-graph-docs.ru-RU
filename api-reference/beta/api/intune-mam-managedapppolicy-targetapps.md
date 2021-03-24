---
title: Действие targetApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9177052eae671fa59036780b416e5910a0c82d8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149235"
---
# <a name="targetapps-action"></a><span data-ttu-id="7db83-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="7db83-103">targetApps action</span></span>

<span data-ttu-id="7db83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7db83-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7db83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7db83-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7db83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7db83-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7db83-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7db83-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7db83-108">Prerequisites</span></span>
<span data-ttu-id="7db83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7db83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7db83-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7db83-111">Permission type</span></span>|<span data-ttu-id="7db83-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7db83-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7db83-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7db83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7db83-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7db83-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7db83-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7db83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7db83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7db83-116">Not supported.</span></span>|
|<span data-ttu-id="7db83-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7db83-117">Application</span></span>|<span data-ttu-id="7db83-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7db83-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7db83-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7db83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="7db83-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7db83-120">Request headers</span></span>
|<span data-ttu-id="7db83-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7db83-121">Header</span></span>|<span data-ttu-id="7db83-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7db83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7db83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7db83-123">Authorization</span></span>|<span data-ttu-id="7db83-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7db83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7db83-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7db83-125">Accept</span></span>|<span data-ttu-id="7db83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7db83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7db83-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7db83-127">Request body</span></span>
<span data-ttu-id="7db83-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7db83-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7db83-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7db83-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7db83-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7db83-130">Property</span></span>|<span data-ttu-id="7db83-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7db83-131">Type</span></span>|<span data-ttu-id="7db83-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7db83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7db83-133">apps</span><span class="sxs-lookup"><span data-stu-id="7db83-133">apps</span></span>|<span data-ttu-id="7db83-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7db83-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="7db83-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="7db83-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7db83-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7db83-136">Response</span></span>
<span data-ttu-id="7db83-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7db83-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7db83-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7db83-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7db83-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7db83-139">Request</span></span>
<span data-ttu-id="7db83-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7db83-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7db83-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7db83-141">Response</span></span>
<span data-ttu-id="7db83-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7db83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




