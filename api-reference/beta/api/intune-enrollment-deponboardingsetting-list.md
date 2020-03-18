---
title: Список depOnboardingSettings
description: Список свойств и связей объектов depOnboardingSetting.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf8537c8754fe445b7f84a61f8f6d152b8920d1d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813241"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="cd99d-103">Список depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="cd99d-103">List depOnboardingSettings</span></span>

> <span data-ttu-id="cd99d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd99d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd99d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd99d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd99d-106">Список свойств и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="cd99d-106">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd99d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd99d-107">Prerequisites</span></span>
<span data-ttu-id="cd99d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd99d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd99d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd99d-110">Permission type</span></span>|<span data-ttu-id="cd99d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd99d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd99d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd99d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd99d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd99d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cd99d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd99d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd99d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd99d-115">Not supported.</span></span>|
|<span data-ttu-id="cd99d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cd99d-116">Application</span></span>|<span data-ttu-id="cd99d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd99d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd99d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd99d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="cd99d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd99d-119">Request headers</span></span>
|<span data-ttu-id="cd99d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd99d-120">Header</span></span>|<span data-ttu-id="cd99d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd99d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd99d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd99d-122">Authorization</span></span>|<span data-ttu-id="cd99d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd99d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd99d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd99d-124">Accept</span></span>|<span data-ttu-id="cd99d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd99d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd99d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd99d-126">Request body</span></span>
<span data-ttu-id="cd99d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd99d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd99d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd99d-128">Response</span></span>
<span data-ttu-id="cd99d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd99d-129">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd99d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cd99d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd99d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd99d-131">Request</span></span>
<span data-ttu-id="cd99d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd99d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="cd99d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd99d-133">Response</span></span>
<span data-ttu-id="cd99d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd99d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depOnboardingSetting",
      "id": "40342229-2229-4034-2922-344029223440",
      "appleIdentifier": "Apple Identifier value",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
      "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
      "shareTokenWithSchoolDataSyncService": true,
      "lastSyncErrorCode": 1,
      "tokenType": "dep",
      "tokenName": "Token Name value",
      "syncedDeviceCount": 1,
      "dataSharingConsentGranted": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




