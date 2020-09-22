---
title: Получение Мобилеаппрелатионшип
description: Чтение свойств и связей объекта Мобилеаппрелатионшип.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee71b987fb8a0ceb2ccaaf4077b9205158ea3f40
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977042"
---
# <a name="get-mobileapprelationship"></a><span data-ttu-id="7376a-103">Получение Мобилеаппрелатионшип</span><span class="sxs-lookup"><span data-stu-id="7376a-103">Get mobileAppRelationship</span></span>

<span data-ttu-id="7376a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7376a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7376a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7376a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7376a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7376a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7376a-107">Чтение свойств и связей объекта [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="7376a-107">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7376a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7376a-108">Prerequisites</span></span>
<span data-ttu-id="7376a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7376a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7376a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7376a-111">Permission type</span></span>|<span data-ttu-id="7376a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7376a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7376a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7376a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7376a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7376a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7376a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7376a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7376a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7376a-116">Not supported.</span></span>|
|<span data-ttu-id="7376a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7376a-117">Application</span></span>|<span data-ttu-id="7376a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7376a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7376a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7376a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7376a-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7376a-120">Optional query parameters</span></span>
<span data-ttu-id="7376a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7376a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7376a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7376a-122">Request headers</span></span>
|<span data-ttu-id="7376a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7376a-123">Header</span></span>|<span data-ttu-id="7376a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7376a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7376a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7376a-125">Authorization</span></span>|<span data-ttu-id="7376a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7376a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7376a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7376a-127">Accept</span></span>|<span data-ttu-id="7376a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7376a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7376a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7376a-129">Request body</span></span>
<span data-ttu-id="7376a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7376a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7376a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7376a-131">Response</span></span>
<span data-ttu-id="7376a-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7376a-132">If successful, this method returns a `200 OK` response code and [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7376a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7376a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7376a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7376a-134">Request</span></span>
<span data-ttu-id="7376a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7376a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="7376a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7376a-136">Response</span></span>
<span data-ttu-id="7376a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7376a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppRelationship",
    "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "targetType": "parent"
  }
}
```






