---
title: Список Мобилеаппрелатионшипс
description: Список свойств и связей объектов Мобилеаппрелатионшип.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3f535fee5e148d492c2c1401fed5a632a9bf5e3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172424"
---
# <a name="list-mobileapprelationships"></a><span data-ttu-id="bab71-103">Список Мобилеаппрелатионшипс</span><span class="sxs-lookup"><span data-stu-id="bab71-103">List mobileAppRelationships</span></span>

> <span data-ttu-id="bab71-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bab71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bab71-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bab71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bab71-106">Список свойств и связей объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="bab71-106">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bab71-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bab71-107">Prerequisites</span></span>
<span data-ttu-id="bab71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab71-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bab71-110">Permission type</span></span>|<span data-ttu-id="bab71-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bab71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bab71-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bab71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bab71-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab71-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bab71-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bab71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab71-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bab71-115">Not supported.</span></span>|
|<span data-ttu-id="bab71-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bab71-116">Application</span></span>|<span data-ttu-id="bab71-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab71-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bab71-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bab71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="bab71-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bab71-119">Request headers</span></span>
|<span data-ttu-id="bab71-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bab71-120">Header</span></span>|<span data-ttu-id="bab71-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bab71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bab71-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bab71-122">Authorization</span></span>|<span data-ttu-id="bab71-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bab71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bab71-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bab71-124">Accept</span></span>|<span data-ttu-id="bab71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bab71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab71-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bab71-126">Request body</span></span>
<span data-ttu-id="bab71-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bab71-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab71-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bab71-128">Response</span></span>
<span data-ttu-id="bab71-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bab71-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bab71-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bab71-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bab71-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bab71-131">Request</span></span>
<span data-ttu-id="bab71-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bab71-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="bab71-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab71-133">Response</span></span>
<span data-ttu-id="bab71-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bab71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value"
    }
  ]
}
```




