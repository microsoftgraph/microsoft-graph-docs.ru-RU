---
title: Перечисление объектов windowsPhone81CompliancePolicy
description: Список свойств и связей объектов windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e6bd59b81739aa740fcc6bbb178db1773afdb52
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965447"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="5f0b7-103">Перечисление объектов windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5f0b7-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="5f0b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f0b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f0b7-106">Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f0b7-106">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f0b7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5f0b7-107">Prerequisites</span></span>
<span data-ttu-id="5f0b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f0b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f0b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f0b7-110">Permission type</span></span>|<span data-ttu-id="5f0b7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f0b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f0b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f0b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f0b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f0b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f0b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f0b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f0b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-115">Not supported.</span></span>|
|<span data-ttu-id="5f0b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f0b7-116">Application</span></span>|<span data-ttu-id="5f0b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f0b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f0b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5f0b7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f0b7-119">Request headers</span></span>
|<span data-ttu-id="5f0b7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f0b7-120">Header</span></span>|<span data-ttu-id="5f0b7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5f0b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f0b7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f0b7-122">Authorization</span></span>|<span data-ttu-id="5f0b7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f0b7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f0b7-124">Accept</span></span>|<span data-ttu-id="5f0b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f0b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f0b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f0b7-126">Request body</span></span>
<span data-ttu-id="5f0b7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f0b7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f0b7-128">Response</span></span>
<span data-ttu-id="5f0b7-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f0b7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5f0b7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f0b7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f0b7-131">Request</span></span>
<span data-ttu-id="5f0b7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="5f0b7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f0b7-133">Response</span></span>
<span data-ttu-id="5f0b7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f0b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
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
  ]
}
```




