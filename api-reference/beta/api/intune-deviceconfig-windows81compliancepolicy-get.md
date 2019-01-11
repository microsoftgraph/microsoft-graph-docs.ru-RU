---
title: Получение windows81CompliancePolicy
description: Чтение свойств и связей объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68d72ff0e8d7a43df7e2622b0781f81b0418a485
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809256"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="51e0a-103">Получение windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="51e0a-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="51e0a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51e0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51e0a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51e0a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51e0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51e0a-107">Чтение свойств и связей объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51e0a-107">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51e0a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51e0a-108">Prerequisites</span></span>
<span data-ttu-id="51e0a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e0a-111">Permission type</span></span>|<span data-ttu-id="51e0a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51e0a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51e0a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51e0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e0a-116">Not supported.</span></span>|
|<span data-ttu-id="51e0a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51e0a-117">Application</span></span>|<span data-ttu-id="51e0a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51e0a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51e0a-120">Optional query parameters</span></span>
<span data-ttu-id="51e0a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51e0a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51e0a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51e0a-122">Request headers</span></span>
|<span data-ttu-id="51e0a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51e0a-123">Header</span></span>|<span data-ttu-id="51e0a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="51e0a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e0a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e0a-125">Authorization</span></span>|<span data-ttu-id="51e0a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51e0a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e0a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="51e0a-127">Accept</span></span>|<span data-ttu-id="51e0a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51e0a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e0a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51e0a-129">Request body</span></span>
<span data-ttu-id="51e0a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51e0a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51e0a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e0a-131">Response</span></span>
<span data-ttu-id="51e0a-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51e0a-132">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e0a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="51e0a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="51e0a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e0a-134">Request</span></span>
<span data-ttu-id="51e0a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e0a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="51e0a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="51e0a-136">Response</span></span>
<span data-ttu-id="51e0a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51e0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





