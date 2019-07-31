---
title: Получение windows81CompliancePolicy
description: Чтение свойств и связей объекта windows81CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cfc07d99296c249a4a8650b7cd3919a161fc776
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975048"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="0c769-103">Получение windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0c769-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="0c769-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c769-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c769-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c769-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c769-106">Чтение свойств и связей объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c769-106">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c769-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0c769-107">Prerequisites</span></span>
<span data-ttu-id="0c769-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c769-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c769-110">Permission type</span></span>|<span data-ttu-id="0c769-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c769-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c769-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c769-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c769-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c769-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0c769-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c769-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c769-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c769-115">Not supported.</span></span>|
|<span data-ttu-id="0c769-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c769-116">Application</span></span>|<span data-ttu-id="0c769-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c769-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c769-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c769-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c769-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c769-119">Optional query parameters</span></span>
<span data-ttu-id="0c769-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c769-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c769-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c769-121">Request headers</span></span>
|<span data-ttu-id="0c769-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c769-122">Header</span></span>|<span data-ttu-id="0c769-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0c769-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c769-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c769-124">Authorization</span></span>|<span data-ttu-id="0c769-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c769-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c769-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0c769-126">Accept</span></span>|<span data-ttu-id="0c769-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c769-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c769-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c769-128">Request body</span></span>
<span data-ttu-id="0c769-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c769-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c769-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c769-130">Response</span></span>
<span data-ttu-id="0c769-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c769-131">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c769-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0c769-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c769-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c769-133">Request</span></span>
<span data-ttu-id="0c769-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c769-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="0c769-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c769-135">Response</span></span>
<span data-ttu-id="0c769-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c769-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





