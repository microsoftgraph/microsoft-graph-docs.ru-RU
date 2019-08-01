---
title: Перечисление объектов windowsPhone81CompliancePolicy
description: Список свойств и связей объектов windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d15b686b5081f60a64091fc7a4c5a96a4223a758
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997099"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="c9d85-103">Перечисление объектов windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c9d85-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="c9d85-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9d85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d85-105">Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9d85-105">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9d85-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9d85-106">Prerequisites</span></span>
<span data-ttu-id="c9d85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d85-109">Permission type</span></span>|<span data-ttu-id="c9d85-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9d85-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9d85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9d85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9d85-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9d85-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9d85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9d85-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9d85-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d85-114">Not supported.</span></span>|
|<span data-ttu-id="c9d85-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9d85-115">Application</span></span>|<span data-ttu-id="c9d85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d85-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9d85-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9d85-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c9d85-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9d85-118">Request headers</span></span>
|<span data-ttu-id="c9d85-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9d85-119">Header</span></span>|<span data-ttu-id="c9d85-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c9d85-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9d85-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9d85-121">Authorization</span></span>|<span data-ttu-id="c9d85-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9d85-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9d85-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c9d85-123">Accept</span></span>|<span data-ttu-id="c9d85-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9d85-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9d85-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9d85-125">Request body</span></span>
<span data-ttu-id="c9d85-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9d85-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9d85-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9d85-127">Response</span></span>
<span data-ttu-id="c9d85-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d85-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d85-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c9d85-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9d85-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9d85-130">Request</span></span>
<span data-ttu-id="c9d85-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9d85-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="c9d85-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d85-132">Response</span></span>
<span data-ttu-id="c9d85-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9d85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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
  ]
}
```



