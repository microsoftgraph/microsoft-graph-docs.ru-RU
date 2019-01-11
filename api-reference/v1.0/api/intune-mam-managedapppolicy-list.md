---
title: Перечисление объектов managedAppPolicy
description: Список свойств и связей объектов managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3169e1a189205049d3a18a578af06b4f1528628b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832685"
---
# <a name="list-managedapppolicies"></a><span data-ttu-id="26c5b-103">Перечисление объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="26c5b-103">List managedAppPolicies</span></span>

> <span data-ttu-id="26c5b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="26c5b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26c5b-105">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26c5b-105">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26c5b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="26c5b-106">Prerequisites</span></span>
<span data-ttu-id="26c5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26c5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26c5b-109">Permission type</span></span>|<span data-ttu-id="26c5b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26c5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26c5b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26c5b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26c5b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="26c5b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="26c5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26c5b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26c5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26c5b-114">Not supported.</span></span>|
|<span data-ttu-id="26c5b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26c5b-115">Application</span></span>|<span data-ttu-id="26c5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26c5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26c5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26c5b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="26c5b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26c5b-118">Request headers</span></span>
|<span data-ttu-id="26c5b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26c5b-119">Header</span></span>|<span data-ttu-id="26c5b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26c5b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26c5b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c5b-121">Authorization</span></span>|<span data-ttu-id="26c5b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="26c5b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26c5b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26c5b-123">Accept</span></span>|<span data-ttu-id="26c5b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26c5b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26c5b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26c5b-125">Request body</span></span>
<span data-ttu-id="26c5b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26c5b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26c5b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="26c5b-127">Response</span></span>
<span data-ttu-id="26c5b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26c5b-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c5b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="26c5b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="26c5b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="26c5b-130">Request</span></span>
<span data-ttu-id="26c5b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26c5b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="26c5b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="26c5b-132">Response</span></span>
<span data-ttu-id="26c5b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26c5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```



