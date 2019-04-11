---
title: Список depOnboardingSettings
description: Список свойств и связей объектов depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2af4f462b47e5e2993f2a688be8cdd8440facf98
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789635"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="f8e80-103">Список depOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="f8e80-103">List depOnboardingSettings</span></span>

> <span data-ttu-id="f8e80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8e80-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8e80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e80-106">Список свойств и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f8e80-106">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e80-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8e80-107">Prerequisites</span></span>
<span data-ttu-id="f8e80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8e80-110">Permission type</span></span>|<span data-ttu-id="f8e80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8e80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8e80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e80-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e80-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f8e80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8e80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e80-115">Not supported.</span></span>|
|<span data-ttu-id="f8e80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8e80-116">Application</span></span>|<span data-ttu-id="f8e80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8e80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="f8e80-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8e80-119">Request headers</span></span>
|<span data-ttu-id="f8e80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8e80-120">Header</span></span>|<span data-ttu-id="f8e80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8e80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e80-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8e80-122">Authorization</span></span>|<span data-ttu-id="f8e80-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8e80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8e80-124">Accept</span></span>|<span data-ttu-id="f8e80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8e80-126">Request body</span></span>
<span data-ttu-id="f8e80-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8e80-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8e80-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8e80-128">Response</span></span>
<span data-ttu-id="f8e80-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8e80-129">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e80-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f8e80-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8e80-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8e80-131">Request</span></span>
<span data-ttu-id="f8e80-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8e80-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="f8e80-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8e80-133">Response</span></span>
<span data-ttu-id="f8e80-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8e80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





