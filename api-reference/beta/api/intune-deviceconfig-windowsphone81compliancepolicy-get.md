---
title: Get windowsPhone81CompliancePolicy
description: Чтение свойств и связей объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2ba662ec66a851f972658f5f278492797d87ab3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978502"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="4f396-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4f396-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="4f396-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f396-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f396-106">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f396-106">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f396-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f396-107">Prerequisites</span></span>
<span data-ttu-id="4f396-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f396-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f396-110">Permission type</span></span>|<span data-ttu-id="4f396-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f396-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f396-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f396-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f396-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f396-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f396-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f396-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f396-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f396-115">Not supported.</span></span>|
|<span data-ttu-id="4f396-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f396-116">Application</span></span>|<span data-ttu-id="4f396-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f396-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f396-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f396-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f396-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f396-119">Optional query parameters</span></span>
<span data-ttu-id="4f396-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f396-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f396-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f396-121">Request headers</span></span>
|<span data-ttu-id="4f396-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f396-122">Header</span></span>|<span data-ttu-id="4f396-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4f396-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f396-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f396-124">Authorization</span></span>|<span data-ttu-id="4f396-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f396-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f396-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4f396-126">Accept</span></span>|<span data-ttu-id="4f396-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4f396-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f396-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f396-128">Request body</span></span>
<span data-ttu-id="4f396-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f396-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f396-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f396-130">Response</span></span>
<span data-ttu-id="4f396-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f396-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f396-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4f396-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f396-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f396-133">Request</span></span>
<span data-ttu-id="4f396-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f396-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4f396-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f396-135">Response</span></span>
<span data-ttu-id="4f396-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f396-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```




