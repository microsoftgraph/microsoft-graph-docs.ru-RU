---
title: Get chromeOSOnboardingSettings
description: Чтение свойств и связей объекта chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d67ea0148e31f4f692c80c0794b3a2b733e2d00e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665966"
---
# <a name="get-chromeosonboardingsettings"></a><span data-ttu-id="0599b-103">Get chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="0599b-103">Get chromeOSOnboardingSettings</span></span>

<span data-ttu-id="0599b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0599b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0599b-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0599b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0599b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0599b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0599b-107">Чтение свойств и связей [объекта chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0599b-107">Read properties and relationships of the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0599b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0599b-108">Prerequisites</span></span>
<span data-ttu-id="0599b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0599b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0599b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0599b-111">Permission type</span></span>|<span data-ttu-id="0599b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0599b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0599b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0599b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0599b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0599b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0599b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0599b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0599b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0599b-116">Not supported.</span></span>|
|<span data-ttu-id="0599b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0599b-117">Application</span></span>|<span data-ttu-id="0599b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0599b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0599b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0599b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0599b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0599b-120">Optional query parameters</span></span>
<span data-ttu-id="0599b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0599b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0599b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0599b-122">Request headers</span></span>
|<span data-ttu-id="0599b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0599b-123">Header</span></span>|<span data-ttu-id="0599b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0599b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0599b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0599b-125">Authorization</span></span>|<span data-ttu-id="0599b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0599b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0599b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0599b-127">Accept</span></span>|<span data-ttu-id="0599b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0599b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0599b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0599b-129">Request body</span></span>
<span data-ttu-id="0599b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0599b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0599b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0599b-131">Response</span></span>
<span data-ttu-id="0599b-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0599b-132">If successful, this method returns a `200 OK` response code and [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0599b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0599b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0599b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0599b-134">Request</span></span>
<span data-ttu-id="0599b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0599b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
```

### <a name="response"></a><span data-ttu-id="0599b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0599b-136">Response</span></span>
<span data-ttu-id="0599b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0599b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": {
    "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
    "id": "0344255d-255d-0344-5d25-44035d254403",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "onboardingStatus": "inprogress",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
  }
}
```




