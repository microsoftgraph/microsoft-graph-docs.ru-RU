---
title: Get windowsQualityUpdateCatalogItem
description: Чтение свойств и связей объекта windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 027c447fa87bc0bfdcf1603756cb5392c2d6dbce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160988"
---
# <a name="get-windowsqualityupdatecatalogitem"></a><span data-ttu-id="6cd48-103">Get windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="6cd48-103">Get windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="6cd48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cd48-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cd48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cd48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cd48-107">Чтение свойств и связей объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6cd48-107">Read properties and relationships of the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cd48-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cd48-108">Prerequisites</span></span>
<span data-ttu-id="6cd48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cd48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cd48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cd48-111">Permission type</span></span>|<span data-ttu-id="6cd48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cd48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cd48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cd48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cd48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cd48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cd48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cd48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cd48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd48-116">Not supported.</span></span>|
|<span data-ttu-id="6cd48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cd48-117">Application</span></span>|<span data-ttu-id="6cd48-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cd48-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cd48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cd48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cd48-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6cd48-120">Optional query parameters</span></span>
<span data-ttu-id="6cd48-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6cd48-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cd48-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cd48-122">Request headers</span></span>
|<span data-ttu-id="6cd48-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cd48-123">Header</span></span>|<span data-ttu-id="6cd48-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6cd48-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cd48-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cd48-125">Authorization</span></span>|<span data-ttu-id="6cd48-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cd48-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cd48-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6cd48-127">Accept</span></span>|<span data-ttu-id="6cd48-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd48-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cd48-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cd48-129">Request body</span></span>
<span data-ttu-id="6cd48-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cd48-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cd48-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cd48-131">Response</span></span>
<span data-ttu-id="6cd48-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6cd48-132">If successful, this method returns a `200 OK` response code and [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd48-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6cd48-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cd48-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cd48-134">Request</span></span>
<span data-ttu-id="6cd48-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cd48-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

### <a name="response"></a><span data-ttu-id="6cd48-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cd48-136">Response</span></span>
<span data-ttu-id="6cd48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cd48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 354

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
    "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
    "displayName": "Display Name value",
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "kbArticleId": "Kb Article Id value",
    "classification": "security",
    "isExpeditable": true
  }
}
```




