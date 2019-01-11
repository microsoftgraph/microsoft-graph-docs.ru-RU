---
title: Получение androidWorkProfileGeneralDeviceConfiguration
description: Чтение свойства и связи объекта androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1ce36a8684a269be92523c590f07b2065673def
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883841"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="558c8-103">Получение androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="558c8-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="558c8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="558c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="558c8-105">Чтение свойства и связи объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="558c8-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="558c8-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="558c8-106">Prerequisites</span></span>
<span data-ttu-id="558c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="558c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="558c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="558c8-109">Permission type</span></span>|<span data-ttu-id="558c8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="558c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="558c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="558c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="558c8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="558c8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="558c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="558c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="558c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="558c8-114">Not supported.</span></span>|
|<span data-ttu-id="558c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="558c8-115">Application</span></span>|<span data-ttu-id="558c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="558c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="558c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="558c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="558c8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="558c8-118">Optional query parameters</span></span>
<span data-ttu-id="558c8-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="558c8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="558c8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="558c8-120">Request headers</span></span>
|<span data-ttu-id="558c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="558c8-121">Header</span></span>|<span data-ttu-id="558c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="558c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="558c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="558c8-123">Authorization</span></span>|<span data-ttu-id="558c8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="558c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="558c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="558c8-125">Accept</span></span>|<span data-ttu-id="558c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="558c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="558c8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="558c8-127">Request body</span></span>
<span data-ttu-id="558c8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="558c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="558c8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="558c8-129">Response</span></span>
<span data-ttu-id="558c8-130">Успешно завершена, этот метод возвращает `200 OK` объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="558c8-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="558c8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="558c8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="558c8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="558c8-132">Request</span></span>
<span data-ttu-id="558c8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="558c8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="558c8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="558c8-134">Response</span></span>
<span data-ttu-id="558c8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="558c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true
  }
}
```



