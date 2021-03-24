---
title: Get windowsFeatureUpdateProfile
description: Чтение свойств и связей объекта windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46131ee1512c47d1d8b1b7afa27f434722566927
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134272"
---
# <a name="get-windowsfeatureupdateprofile"></a><span data-ttu-id="49df6-103">Get windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="49df6-103">Get windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="49df6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49df6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49df6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49df6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49df6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49df6-107">Чтение свойств и связей [объекта windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="49df6-107">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49df6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49df6-108">Prerequisites</span></span>
<span data-ttu-id="49df6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49df6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49df6-111">Permission type</span></span>|<span data-ttu-id="49df6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49df6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49df6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49df6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49df6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49df6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49df6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49df6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49df6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49df6-116">Not supported.</span></span>|
|<span data-ttu-id="49df6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="49df6-117">Application</span></span>|<span data-ttu-id="49df6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49df6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49df6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49df6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49df6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49df6-120">Optional query parameters</span></span>
<span data-ttu-id="49df6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49df6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49df6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49df6-122">Request headers</span></span>
|<span data-ttu-id="49df6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49df6-123">Header</span></span>|<span data-ttu-id="49df6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="49df6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49df6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="49df6-125">Authorization</span></span>|<span data-ttu-id="49df6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49df6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49df6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="49df6-127">Accept</span></span>|<span data-ttu-id="49df6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="49df6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49df6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49df6-129">Request body</span></span>
<span data-ttu-id="49df6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49df6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49df6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="49df6-131">Response</span></span>
<span data-ttu-id="49df6-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49df6-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49df6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="49df6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="49df6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="49df6-134">Request</span></span>
<span data-ttu-id="49df6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49df6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

### <a name="response"></a><span data-ttu-id="49df6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="49df6-136">Response</span></span>
<span data-ttu-id="49df6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49df6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
    "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
    "displayName": "Display Name value",
    "description": "Description value",
    "featureUpdateVersion": "Feature Update Version value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "deployableContentDisplayName": "Deployable Content Display Name value"
  }
}
```




