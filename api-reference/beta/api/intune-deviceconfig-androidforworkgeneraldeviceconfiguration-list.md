---
title: Список androidForWorkGeneralDeviceConfigurations
description: Свойства списка и связей объектов androidForWorkGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aec8814e6617ef713bdc515cd77b4a983a405fa6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813008"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="8cab6-103">Список androidForWorkGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="8cab6-103">List androidForWorkGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="8cab6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cab6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cab6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cab6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cab6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8cab6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cab6-107">Свойства списка и связей объектов [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8cab6-107">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cab6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cab6-108">Prerequisites</span></span>
<span data-ttu-id="8cab6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cab6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cab6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cab6-111">Permission type</span></span>|<span data-ttu-id="8cab6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cab6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cab6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cab6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cab6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cab6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8cab6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cab6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cab6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cab6-116">Not supported.</span></span>|
|<span data-ttu-id="8cab6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cab6-117">Application</span></span>|<span data-ttu-id="8cab6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cab6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cab6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cab6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8cab6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cab6-120">Request headers</span></span>
|<span data-ttu-id="8cab6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cab6-121">Header</span></span>|<span data-ttu-id="8cab6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cab6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cab6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cab6-123">Authorization</span></span>|<span data-ttu-id="8cab6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8cab6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cab6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cab6-125">Accept</span></span>|<span data-ttu-id="8cab6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cab6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cab6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8cab6-127">Request body</span></span>
<span data-ttu-id="8cab6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cab6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cab6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cab6-129">Response</span></span>
<span data-ttu-id="8cab6-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8cab6-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cab6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8cab6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cab6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cab6-132">Request</span></span>
<span data-ttu-id="8cab6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cab6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8cab6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cab6-134">Response</span></span>
<span data-ttu-id="8cab6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8cab6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2431

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
      "id": "a931a366-a366-a931-66a3-31a966a331a9",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "securityRequireVerifyApps": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnEnableAlwaysOnLockdownMode": true
    }
  ]
}
```





