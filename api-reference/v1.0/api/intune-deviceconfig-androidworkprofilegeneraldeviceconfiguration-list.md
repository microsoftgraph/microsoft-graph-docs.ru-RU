---
title: Список Андроидворкпрофилеженералдевицеконфигуратионс
description: Список свойств и связей объектов androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f821208383f6dece05433f8541e5be2fcfc3acd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250784"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="36a1a-103">Список Андроидворкпрофилеженералдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="36a1a-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="36a1a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36a1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a1a-105">Список свойств и связей объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="36a1a-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36a1a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36a1a-106">Prerequisites</span></span>
<span data-ttu-id="36a1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="36a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36a1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36a1a-109">Permission type</span></span>|<span data-ttu-id="36a1a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36a1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36a1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36a1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36a1a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36a1a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36a1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36a1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36a1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a1a-114">Not supported.</span></span>|
|<span data-ttu-id="36a1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36a1a-115">Application</span></span>|<span data-ttu-id="36a1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36a1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36a1a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36a1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36a1a-118">Request headers</span></span>
|<span data-ttu-id="36a1a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36a1a-119">Header</span></span>|<span data-ttu-id="36a1a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="36a1a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36a1a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36a1a-121">Authorization</span></span>|<span data-ttu-id="36a1a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36a1a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36a1a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="36a1a-123">Accept</span></span>|<span data-ttu-id="36a1a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36a1a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36a1a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36a1a-125">Request body</span></span>
<span data-ttu-id="36a1a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36a1a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36a1a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="36a1a-127">Response</span></span>
<span data-ttu-id="36a1a-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36a1a-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a1a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36a1a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="36a1a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36a1a-130">Request</span></span>
<span data-ttu-id="36a1a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36a1a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="36a1a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="36a1a-132">Response</span></span>
<span data-ttu-id="36a1a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36a1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



