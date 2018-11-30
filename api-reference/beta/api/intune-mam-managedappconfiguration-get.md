---
title: Get managedAppConfiguration
description: Чтение свойств и связей объекта managedAppConfiguration.
ms.openlocfilehash: 12d19046fc3e7fdd3f6ca30efc5c61b965aecd69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079192"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="8337b-103">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8337b-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="8337b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8337b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8337b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8337b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8337b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8337b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8337b-107">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8337b-107">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8337b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8337b-108">Prerequisites</span></span>
<span data-ttu-id="8337b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8337b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8337b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8337b-111">Permission type</span></span>|<span data-ttu-id="8337b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8337b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8337b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8337b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8337b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8337b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8337b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8337b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8337b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8337b-116">Not supported.</span></span>|
|<span data-ttu-id="8337b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8337b-117">Application</span></span>|<span data-ttu-id="8337b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8337b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8337b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8337b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8337b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8337b-120">Optional query parameters</span></span>
<span data-ttu-id="8337b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8337b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8337b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8337b-122">Request headers</span></span>
|<span data-ttu-id="8337b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8337b-123">Header</span></span>|<span data-ttu-id="8337b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8337b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8337b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8337b-125">Authorization</span></span>|<span data-ttu-id="8337b-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8337b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8337b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8337b-127">Accept</span></span>|<span data-ttu-id="8337b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8337b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8337b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8337b-129">Request body</span></span>
<span data-ttu-id="8337b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8337b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8337b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8337b-131">Response</span></span>
<span data-ttu-id="8337b-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8337b-132">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8337b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8337b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8337b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8337b-134">Request</span></span>
<span data-ttu-id="8337b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8337b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="8337b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8337b-136">Response</span></span>
<span data-ttu-id="8337b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8337b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```





