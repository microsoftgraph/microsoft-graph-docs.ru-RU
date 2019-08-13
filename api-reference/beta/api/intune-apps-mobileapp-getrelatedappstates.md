---
title: Функция Жетрелатедаппстатес
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd10d0b2b8dde194c6aa394deec081d2966b1d49
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329364"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="8f1b6-103">Функция Жетрелатедаппстатес</span><span class="sxs-lookup"><span data-stu-id="8f1b6-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="8f1b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f1b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f1b6-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f1b6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f1b6-107">Prerequisites</span></span>
<span data-ttu-id="8f1b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f1b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f1b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f1b6-110">Permission type</span></span>|<span data-ttu-id="8f1b6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f1b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f1b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f1b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f1b6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f1b6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f1b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f1b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f1b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-115">Not supported.</span></span>|
|<span data-ttu-id="8f1b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f1b6-116">Application</span></span>|<span data-ttu-id="8f1b6-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f1b6-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f1b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f1b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="8f1b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f1b6-119">Request headers</span></span>
|<span data-ttu-id="8f1b6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f1b6-120">Header</span></span>|<span data-ttu-id="8f1b6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8f1b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f1b6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f1b6-122">Authorization</span></span>|<span data-ttu-id="8f1b6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f1b6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8f1b6-124">Accept</span></span>|<span data-ttu-id="8f1b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f1b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f1b6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f1b6-126">Request body</span></span>
<span data-ttu-id="8f1b6-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8f1b6-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8f1b6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f1b6-129">Property</span></span>|<span data-ttu-id="8f1b6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f1b6-130">Type</span></span>|<span data-ttu-id="8f1b6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f1b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1b6-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f1b6-132">userPrincipalName</span></span>|<span data-ttu-id="8f1b6-133">String</span><span class="sxs-lookup"><span data-stu-id="8f1b6-133">String</span></span>|<span data-ttu-id="8f1b6-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-134">Not yet documented</span></span>|
|<span data-ttu-id="8f1b6-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="8f1b6-135">deviceId</span></span>|<span data-ttu-id="8f1b6-136">String</span><span class="sxs-lookup"><span data-stu-id="8f1b6-136">String</span></span>|<span data-ttu-id="8f1b6-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8f1b6-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8f1b6-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f1b6-138">Response</span></span>
<span data-ttu-id="8f1b6-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [мобилеаппрелатионшипстате](../resources/intune-apps-mobileapprelationshipstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-139">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f1b6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8f1b6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f1b6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f1b6-141">Request</span></span>
<span data-ttu-id="8f1b6-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8f1b6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f1b6-143">Response</span></span>
<span data-ttu-id="8f1b6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f1b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






