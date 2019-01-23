---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d41cd3ad6b27ab83e5ca0cf97cdeb4e8068b903c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423260"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="16617-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="16617-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="16617-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16617-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16617-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16617-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16617-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16617-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16617-107">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="16617-107">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16617-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16617-108">Prerequisites</span></span>
<span data-ttu-id="16617-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="16617-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16617-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16617-111">Permission type</span></span>|<span data-ttu-id="16617-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16617-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16617-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16617-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16617-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16617-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="16617-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16617-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16617-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16617-116">Not supported.</span></span>|
|<span data-ttu-id="16617-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16617-117">Application</span></span>|<span data-ttu-id="16617-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16617-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16617-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16617-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="16617-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16617-120">Request headers</span></span>
|<span data-ttu-id="16617-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16617-121">Header</span></span>|<span data-ttu-id="16617-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16617-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16617-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16617-123">Authorization</span></span>|<span data-ttu-id="16617-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16617-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16617-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16617-125">Accept</span></span>|<span data-ttu-id="16617-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16617-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16617-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16617-127">Request body</span></span>
<span data-ttu-id="16617-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16617-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16617-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16617-129">Response</span></span>
<span data-ttu-id="16617-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16617-130">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16617-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16617-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="16617-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16617-132">Request</span></span>
<span data-ttu-id="16617-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16617-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="16617-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="16617-134">Response</span></span>
<span data-ttu-id="16617-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16617-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 953

{
  "value": [
    {
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
  ]
}
```




