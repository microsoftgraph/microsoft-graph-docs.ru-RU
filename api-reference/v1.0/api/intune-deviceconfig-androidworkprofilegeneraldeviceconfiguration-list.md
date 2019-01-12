---
title: Список androidWorkProfileGeneralDeviceConfigurations
description: Свойства списка и связей объектов androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bba0ef30142afa2e033606f613d7748046a076a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929741"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="1ed13-103">Список androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="1ed13-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="1ed13-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ed13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ed13-105">Свойства списка и связей объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed13-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ed13-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ed13-106">Prerequisites</span></span>
<span data-ttu-id="1ed13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed13-109">Permission type</span></span>|<span data-ttu-id="1ed13-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ed13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ed13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed13-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ed13-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ed13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ed13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed13-114">Not supported.</span></span>|
|<span data-ttu-id="1ed13-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ed13-115">Application</span></span>|<span data-ttu-id="1ed13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed13-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ed13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ed13-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ed13-118">Request headers</span></span>
|<span data-ttu-id="1ed13-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ed13-119">Header</span></span>|<span data-ttu-id="1ed13-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1ed13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ed13-121">Authorization</span></span>|<span data-ttu-id="1ed13-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1ed13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed13-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1ed13-123">Accept</span></span>|<span data-ttu-id="1ed13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed13-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ed13-125">Request body</span></span>
<span data-ttu-id="1ed13-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ed13-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ed13-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ed13-127">Response</span></span>
<span data-ttu-id="1ed13-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1ed13-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed13-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1ed13-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ed13-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ed13-130">Request</span></span>
<span data-ttu-id="1ed13-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ed13-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1ed13-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ed13-132">Response</span></span>
<span data-ttu-id="1ed13-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ed13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": [
    {
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
  ]
}
```



