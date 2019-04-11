---
title: Получение depOnboardingSetting
description: Чтение свойств и связей объекта depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 933cd6c2ed0e11f1230f532499cb21483f5c25ff
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800170"
---
# <a name="get-deponboardingsetting"></a><span data-ttu-id="712af-103">Получение depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="712af-103">Get depOnboardingSetting</span></span>

> <span data-ttu-id="712af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="712af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="712af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="712af-106">Чтение свойств и связей объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="712af-106">Read properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="712af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="712af-107">Prerequisites</span></span>
<span data-ttu-id="712af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="712af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="712af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="712af-110">Permission type</span></span>|<span data-ttu-id="712af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="712af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="712af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="712af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="712af-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="712af-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="712af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="712af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="712af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712af-115">Not supported.</span></span>|
|<span data-ttu-id="712af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="712af-116">Application</span></span>|<span data-ttu-id="712af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="712af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="712af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="712af-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="712af-119">Optional query parameters</span></span>
<span data-ttu-id="712af-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="712af-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="712af-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="712af-121">Request headers</span></span>
|<span data-ttu-id="712af-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="712af-122">Header</span></span>|<span data-ttu-id="712af-123">Значение</span><span class="sxs-lookup"><span data-stu-id="712af-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="712af-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="712af-124">Authorization</span></span>|<span data-ttu-id="712af-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="712af-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="712af-126">Accept</span><span class="sxs-lookup"><span data-stu-id="712af-126">Accept</span></span>|<span data-ttu-id="712af-127">application/json</span><span class="sxs-lookup"><span data-stu-id="712af-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="712af-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="712af-128">Request body</span></span>
<span data-ttu-id="712af-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="712af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="712af-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="712af-130">Response</span></span>
<span data-ttu-id="712af-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="712af-131">If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="712af-132">Пример</span><span class="sxs-lookup"><span data-stu-id="712af-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="712af-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="712af-133">Request</span></span>
<span data-ttu-id="712af-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="712af-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### <a name="response"></a><span data-ttu-id="712af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="712af-135">Response</span></span>
<span data-ttu-id="712af-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="712af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 740

{
  "value": {
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
}
```





