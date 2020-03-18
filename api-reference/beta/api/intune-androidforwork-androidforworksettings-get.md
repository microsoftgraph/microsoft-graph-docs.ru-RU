---
title: Get androidForWorkSettings
description: Чтение свойств и связей объекта androidForWorkSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c92e744790228dc3e9018b8b2d1c887ab5b7138
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815679"
---
# <a name="get-androidforworksettings"></a><span data-ttu-id="efa73-103">Get androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="efa73-103">Get androidForWorkSettings</span></span>

> <span data-ttu-id="efa73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa73-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efa73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa73-106">Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="efa73-106">Read properties and relationships of the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efa73-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="efa73-107">Prerequisites</span></span>
<span data-ttu-id="efa73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efa73-110">Permission type</span></span>|<span data-ttu-id="efa73-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efa73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efa73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efa73-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="efa73-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="efa73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efa73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa73-115">Not supported.</span></span>|
|<span data-ttu-id="efa73-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="efa73-116">Application</span></span>|<span data-ttu-id="efa73-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="efa73-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efa73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efa73-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efa73-119">Optional query parameters</span></span>
<span data-ttu-id="efa73-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="efa73-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efa73-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efa73-121">Request headers</span></span>
|<span data-ttu-id="efa73-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efa73-122">Header</span></span>|<span data-ttu-id="efa73-123">Значение</span><span class="sxs-lookup"><span data-stu-id="efa73-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa73-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="efa73-124">Authorization</span></span>|<span data-ttu-id="efa73-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efa73-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa73-126">Accept</span><span class="sxs-lookup"><span data-stu-id="efa73-126">Accept</span></span>|<span data-ttu-id="efa73-127">application/json</span><span class="sxs-lookup"><span data-stu-id="efa73-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa73-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efa73-128">Request body</span></span>
<span data-ttu-id="efa73-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efa73-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efa73-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="efa73-130">Response</span></span>
<span data-ttu-id="efa73-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="efa73-131">If successful, this method returns a `200 OK` response code and [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa73-132">Пример</span><span class="sxs-lookup"><span data-stu-id="efa73-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="efa73-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="efa73-133">Request</span></span>
<span data-ttu-id="efa73-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efa73-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
```

### <a name="response"></a><span data-ttu-id="efa73-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa73-135">Response</span></span>
<span data-ttu-id="efa73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efa73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkSettings",
    "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true
  }
}
```




