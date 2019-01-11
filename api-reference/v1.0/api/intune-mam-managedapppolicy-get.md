---
title: Get managedAppPolicy
description: Чтение свойств и связей объекта managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: de7f194aa6d8d47fe9944a08689d2b5bb9e83cf8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886452"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="da304-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="da304-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="da304-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="da304-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da304-105">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="da304-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da304-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="da304-106">Prerequisites</span></span>
<span data-ttu-id="da304-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da304-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da304-109">Permission type</span></span>|<span data-ttu-id="da304-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da304-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da304-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da304-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da304-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da304-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da304-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da304-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da304-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da304-114">Not supported.</span></span>|
|<span data-ttu-id="da304-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da304-115">Application</span></span>|<span data-ttu-id="da304-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da304-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da304-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da304-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da304-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da304-118">Optional query parameters</span></span>
<span data-ttu-id="da304-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da304-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da304-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da304-120">Request headers</span></span>
|<span data-ttu-id="da304-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da304-121">Header</span></span>|<span data-ttu-id="da304-122">Значение</span><span class="sxs-lookup"><span data-stu-id="da304-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da304-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da304-123">Authorization</span></span>|<span data-ttu-id="da304-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="da304-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da304-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da304-125">Accept</span></span>|<span data-ttu-id="da304-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da304-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da304-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da304-127">Request body</span></span>
<span data-ttu-id="da304-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da304-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da304-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="da304-129">Response</span></span>
<span data-ttu-id="da304-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="da304-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da304-131">Пример</span><span class="sxs-lookup"><span data-stu-id="da304-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da304-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="da304-132">Request</span></span>
<span data-ttu-id="da304-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da304-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="da304-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="da304-134">Response</span></span>
<span data-ttu-id="da304-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da304-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```



