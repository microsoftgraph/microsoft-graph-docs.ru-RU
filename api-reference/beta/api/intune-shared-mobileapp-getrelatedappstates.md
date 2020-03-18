---
title: Функция Жетрелатедаппстатес
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e47d77235ca2ca146e6f87d8a619b418e9a6d68
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800790"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="02c81-103">Функция Жетрелатедаппстатес</span><span class="sxs-lookup"><span data-stu-id="02c81-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="02c81-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02c81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02c81-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02c81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02c81-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="02c81-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02c81-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="02c81-107">Prerequisites</span></span>
<span data-ttu-id="02c81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02c81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02c81-110">Permission type</span></span>|<span data-ttu-id="02c81-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02c81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02c81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02c81-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="02c81-113">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="02c81-113">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="02c81-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02c81-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="02c81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02c81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02c81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02c81-116">Not supported.</span></span>|
|<span data-ttu-id="02c81-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="02c81-117">Application</span></span>||
| <span data-ttu-id="02c81-118">&nbsp;&nbsp; **Приложения)**</span><span class="sxs-lookup"><span data-stu-id="02c81-118">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="02c81-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02c81-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02c81-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02c81-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="02c81-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02c81-121">Request headers</span></span>
|<span data-ttu-id="02c81-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02c81-122">Header</span></span>|<span data-ttu-id="02c81-123">Значение</span><span class="sxs-lookup"><span data-stu-id="02c81-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02c81-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02c81-124">Authorization</span></span>|<span data-ttu-id="02c81-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02c81-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02c81-126">Accept</span><span class="sxs-lookup"><span data-stu-id="02c81-126">Accept</span></span>|<span data-ttu-id="02c81-127">application/json</span><span class="sxs-lookup"><span data-stu-id="02c81-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02c81-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02c81-128">Request body</span></span>
<span data-ttu-id="02c81-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="02c81-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="02c81-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="02c81-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="02c81-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c81-131">Property</span></span>|<span data-ttu-id="02c81-132">Тип</span><span class="sxs-lookup"><span data-stu-id="02c81-132">Type</span></span>|<span data-ttu-id="02c81-133">Описание</span><span class="sxs-lookup"><span data-stu-id="02c81-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02c81-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02c81-134">userPrincipalName</span></span>|<span data-ttu-id="02c81-135">String</span><span class="sxs-lookup"><span data-stu-id="02c81-135">String</span></span>|<span data-ttu-id="02c81-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="02c81-136">Not yet documented</span></span>|
|<span data-ttu-id="02c81-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="02c81-137">deviceId</span></span>|<span data-ttu-id="02c81-138">String</span><span class="sxs-lookup"><span data-stu-id="02c81-138">String</span></span>|<span data-ttu-id="02c81-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="02c81-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="02c81-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="02c81-140">Response</span></span>
<span data-ttu-id="02c81-141">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [мобилеаппрелатионшипстате](../resources/intune-apps-mobileapprelationshipstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02c81-141">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02c81-142">Пример</span><span class="sxs-lookup"><span data-stu-id="02c81-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="02c81-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="02c81-143">Request</span></span>
<span data-ttu-id="02c81-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02c81-144">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="02c81-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="02c81-145">Response</span></span>
<span data-ttu-id="02c81-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02c81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState",
      "sourceIds": [
        "Source Ids value"
      ],
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "deviceId": "Device Id value",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "targetLastSyncDateTime": "2017-01-01T00:02:09.7809949-08:00"
    }
  ]
}
```







