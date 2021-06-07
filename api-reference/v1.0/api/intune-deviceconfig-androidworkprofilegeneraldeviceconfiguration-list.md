---
title: Список androidWorkProfileGeneralDeviceConfigurations
description: Список свойств и связей объектов AndroidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cf68e465011d122a8b346a1a45a1ca38750aa04
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757145"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="866b6-103">Список androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="866b6-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

<span data-ttu-id="866b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="866b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="866b6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="866b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="866b6-106">Список свойств и связей объектов [AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="866b6-106">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="866b6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="866b6-107">Prerequisites</span></span>
<span data-ttu-id="866b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="866b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="866b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="866b6-110">Permission type</span></span>|<span data-ttu-id="866b6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="866b6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="866b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="866b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="866b6-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866b6-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="866b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="866b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="866b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866b6-115">Not supported.</span></span>|
|<span data-ttu-id="866b6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="866b6-116">Application</span></span>|<span data-ttu-id="866b6-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866b6-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="866b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="866b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="866b6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="866b6-119">Request headers</span></span>
|<span data-ttu-id="866b6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="866b6-120">Header</span></span>|<span data-ttu-id="866b6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="866b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="866b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="866b6-122">Authorization</span></span>|<span data-ttu-id="866b6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="866b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="866b6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="866b6-124">Accept</span></span>|<span data-ttu-id="866b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="866b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="866b6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="866b6-126">Request body</span></span>
<span data-ttu-id="866b6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="866b6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="866b6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="866b6-128">Response</span></span>
<span data-ttu-id="866b6-129">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="866b6-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="866b6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="866b6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="866b6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="866b6-131">Request</span></span>
<span data-ttu-id="866b6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="866b6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="866b6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="866b6-133">Response</span></span>
<span data-ttu-id="866b6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="866b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




