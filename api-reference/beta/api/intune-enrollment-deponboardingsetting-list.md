---
title: Список depOnboardingSettings
description: Список свойств и связей объектов depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bfe1a1c208236cfa9e9512c4d965abb11bf840a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135693"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="17740-103">Список depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="17740-103">List depOnboardingSettings</span></span>

<span data-ttu-id="17740-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17740-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17740-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17740-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17740-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17740-107">Список свойств и связей объектов [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)</span><span class="sxs-lookup"><span data-stu-id="17740-107">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17740-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17740-108">Prerequisites</span></span>
<span data-ttu-id="17740-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17740-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17740-111">Permission type</span></span>|<span data-ttu-id="17740-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17740-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17740-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17740-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17740-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="17740-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17740-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17740-116">Not supported.</span></span>|
|<span data-ttu-id="17740-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17740-117">Application</span></span>|<span data-ttu-id="17740-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17740-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17740-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="17740-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17740-120">Request headers</span></span>
|<span data-ttu-id="17740-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17740-121">Header</span></span>|<span data-ttu-id="17740-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17740-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17740-123">Authorization</span></span>|<span data-ttu-id="17740-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17740-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17740-125">Accept</span></span>|<span data-ttu-id="17740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17740-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17740-127">Request body</span></span>
<span data-ttu-id="17740-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17740-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17740-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="17740-129">Response</span></span>
<span data-ttu-id="17740-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="17740-130">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17740-131">Пример</span><span class="sxs-lookup"><span data-stu-id="17740-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="17740-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="17740-132">Request</span></span>
<span data-ttu-id="17740-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17740-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="17740-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="17740-134">Response</span></span>
<span data-ttu-id="17740-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17740-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




