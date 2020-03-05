---
title: Список depOnboardingSettings
description: Список свойств и связей объектов depOnboardingSetting.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: caf74dc4925171dd6b8b7b4a2daf7999e78810fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467041"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="5c85f-103">Список depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="5c85f-103">List depOnboardingSettings</span></span>

<span data-ttu-id="5c85f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c85f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c85f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c85f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c85f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c85f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c85f-107">Список свойств и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="5c85f-107">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c85f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c85f-108">Prerequisites</span></span>
<span data-ttu-id="5c85f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c85f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c85f-111">Permission type</span></span>|<span data-ttu-id="5c85f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c85f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c85f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c85f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c85f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c85f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5c85f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c85f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c85f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c85f-116">Not supported.</span></span>|
|<span data-ttu-id="5c85f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c85f-117">Application</span></span>|<span data-ttu-id="5c85f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c85f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c85f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c85f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="5c85f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c85f-120">Request headers</span></span>
|<span data-ttu-id="5c85f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c85f-121">Header</span></span>|<span data-ttu-id="5c85f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5c85f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c85f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c85f-123">Authorization</span></span>|<span data-ttu-id="5c85f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c85f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c85f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c85f-125">Accept</span></span>|<span data-ttu-id="5c85f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c85f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c85f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c85f-127">Request body</span></span>
<span data-ttu-id="5c85f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c85f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c85f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c85f-129">Response</span></span>
<span data-ttu-id="5c85f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c85f-130">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c85f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5c85f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c85f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c85f-132">Request</span></span>
<span data-ttu-id="5c85f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c85f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="5c85f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c85f-134">Response</span></span>
<span data-ttu-id="5c85f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c85f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





