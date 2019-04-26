---
title: Действие targetApps
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b12a463964d2632da670af3784a7364115862b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570927"
---
# <a name="targetapps-action"></a><span data-ttu-id="9dc43-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="9dc43-103">targetApps action</span></span>

> <span data-ttu-id="9dc43-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dc43-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dc43-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9dc43-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dc43-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9dc43-106">Prerequisites</span></span>
<span data-ttu-id="9dc43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dc43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dc43-109">Permission type</span></span>|<span data-ttu-id="9dc43-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dc43-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dc43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dc43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9dc43-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc43-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9dc43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dc43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dc43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc43-114">Not supported.</span></span>|
|<span data-ttu-id="9dc43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dc43-115">Application</span></span>|<span data-ttu-id="9dc43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc43-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dc43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dc43-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="9dc43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dc43-118">Request headers</span></span>
|<span data-ttu-id="9dc43-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dc43-119">Header</span></span>|<span data-ttu-id="9dc43-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9dc43-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dc43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dc43-121">Authorization</span></span>|<span data-ttu-id="9dc43-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dc43-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dc43-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9dc43-123">Accept</span></span>|<span data-ttu-id="9dc43-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9dc43-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dc43-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dc43-125">Request body</span></span>
<span data-ttu-id="9dc43-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dc43-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9dc43-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9dc43-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9dc43-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dc43-128">Property</span></span>|<span data-ttu-id="9dc43-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc43-129">Type</span></span>|<span data-ttu-id="9dc43-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc43-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dc43-131">apps</span><span class="sxs-lookup"><span data-stu-id="9dc43-131">apps</span></span>|<span data-ttu-id="9dc43-132">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9dc43-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="9dc43-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9dc43-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9dc43-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dc43-134">Response</span></span>
<span data-ttu-id="9dc43-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9dc43-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9dc43-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9dc43-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dc43-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dc43-137">Request</span></span>
<span data-ttu-id="9dc43-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dc43-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="9dc43-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc43-139">Response</span></span>
<span data-ttu-id="9dc43-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dc43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



