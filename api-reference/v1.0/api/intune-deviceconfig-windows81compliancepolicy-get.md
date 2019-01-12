---
title: Получение windows81CompliancePolicy
description: Чтение свойств и связей объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3dd288cf60538a623b29f42766f59af76b2c17f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947039"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="96449-103">Получение windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="96449-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="96449-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96449-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96449-105">Чтение свойств и связей объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96449-105">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96449-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="96449-106">Prerequisites</span></span>
<span data-ttu-id="96449-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96449-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96449-109">Permission type</span></span>|<span data-ttu-id="96449-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96449-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96449-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96449-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96449-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96449-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96449-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96449-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96449-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96449-114">Not supported.</span></span>|
|<span data-ttu-id="96449-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96449-115">Application</span></span>|<span data-ttu-id="96449-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96449-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96449-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96449-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96449-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96449-118">Optional query parameters</span></span>
<span data-ttu-id="96449-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96449-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96449-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96449-120">Request headers</span></span>
|<span data-ttu-id="96449-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96449-121">Header</span></span>|<span data-ttu-id="96449-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96449-123">Authorization</span></span>|<span data-ttu-id="96449-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="96449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96449-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96449-125">Accept</span></span>|<span data-ttu-id="96449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96449-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96449-127">Request body</span></span>
<span data-ttu-id="96449-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96449-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96449-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="96449-129">Response</span></span>
<span data-ttu-id="96449-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96449-130">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96449-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96449-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="96449-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96449-132">Request</span></span>
<span data-ttu-id="96449-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96449-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="96449-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="96449-134">Response</span></span>
<span data-ttu-id="96449-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96449-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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



