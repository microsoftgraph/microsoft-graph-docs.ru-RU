---
title: Действие targetApps
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3751dde9dcb54cffdfacd7a186ed8be7545869a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835842"
---
# <a name="targetapps-action"></a><span data-ttu-id="83cd3-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="83cd3-103">targetApps action</span></span>

> <span data-ttu-id="83cd3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="83cd3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83cd3-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="83cd3-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83cd3-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="83cd3-106">Prerequisites</span></span>
<span data-ttu-id="83cd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83cd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83cd3-109">Permission type</span></span>|<span data-ttu-id="83cd3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83cd3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83cd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83cd3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83cd3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83cd3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83cd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83cd3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83cd3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83cd3-114">Not supported.</span></span>|
|<span data-ttu-id="83cd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83cd3-115">Application</span></span>|<span data-ttu-id="83cd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83cd3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83cd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83cd3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="83cd3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83cd3-118">Request headers</span></span>
|<span data-ttu-id="83cd3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83cd3-119">Header</span></span>|<span data-ttu-id="83cd3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="83cd3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83cd3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83cd3-121">Authorization</span></span>|<span data-ttu-id="83cd3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="83cd3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83cd3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83cd3-123">Accept</span></span>|<span data-ttu-id="83cd3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83cd3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83cd3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83cd3-125">Request body</span></span>
<span data-ttu-id="83cd3-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83cd3-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="83cd3-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="83cd3-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="83cd3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="83cd3-128">Property</span></span>|<span data-ttu-id="83cd3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="83cd3-129">Type</span></span>|<span data-ttu-id="83cd3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="83cd3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83cd3-131">apps</span><span class="sxs-lookup"><span data-stu-id="83cd3-131">apps</span></span>|<span data-ttu-id="83cd3-132">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83cd3-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="83cd3-133">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="83cd3-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83cd3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="83cd3-134">Response</span></span>
<span data-ttu-id="83cd3-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83cd3-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83cd3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="83cd3-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="83cd3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="83cd3-137">Request</span></span>
<span data-ttu-id="83cd3-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83cd3-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83cd3-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="83cd3-139">Response</span></span>
<span data-ttu-id="83cd3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="83cd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



