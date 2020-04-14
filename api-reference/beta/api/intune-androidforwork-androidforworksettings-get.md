---
title: Get androidForWorkSettings
description: Чтение свойств и связей объекта androidForWorkSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f80d7cd0b0c56274018645872bd81e2e0bfb59e4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395701"
---
# <a name="get-androidforworksettings"></a><span data-ttu-id="8d637-103">Get androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="8d637-103">Get androidForWorkSettings</span></span>

<span data-ttu-id="8d637-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d637-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d637-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d637-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d637-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d637-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d637-107">Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="8d637-107">Read properties and relationships of the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d637-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8d637-108">Prerequisites</span></span>
<span data-ttu-id="8d637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d637-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d637-111">Permission type</span></span>|<span data-ttu-id="8d637-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d637-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d637-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d637-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d637-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d637-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d637-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d637-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d637-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d637-116">Not supported.</span></span>|
|<span data-ttu-id="8d637-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8d637-117">Application</span></span>|<span data-ttu-id="8d637-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d637-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d637-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d637-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d637-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d637-120">Optional query parameters</span></span>
<span data-ttu-id="8d637-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d637-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d637-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d637-122">Request headers</span></span>
|<span data-ttu-id="8d637-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d637-123">Header</span></span>|<span data-ttu-id="8d637-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8d637-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d637-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d637-125">Authorization</span></span>|<span data-ttu-id="8d637-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d637-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d637-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8d637-127">Accept</span></span>|<span data-ttu-id="8d637-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8d637-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d637-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d637-129">Request body</span></span>
<span data-ttu-id="8d637-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d637-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d637-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d637-131">Response</span></span>
<span data-ttu-id="8d637-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d637-132">If successful, this method returns a `200 OK` response code and [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d637-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8d637-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d637-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d637-134">Request</span></span>
<span data-ttu-id="8d637-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d637-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
```

### <a name="response"></a><span data-ttu-id="8d637-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d637-136">Response</span></span>
<span data-ttu-id="8d637-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d637-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



