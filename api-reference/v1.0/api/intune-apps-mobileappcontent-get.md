---
title: Get mobileAppContent
description: Чтение свойств и связей объекта mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a95baf3d2d07af5f876abd2e7ec6f8a496785232
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982786"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="7fb24-103">Get mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7fb24-103">Get mobileAppContent</span></span>

> <span data-ttu-id="7fb24-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fb24-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fb24-105">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7fb24-105">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fb24-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb24-106">Prerequisites</span></span>
<span data-ttu-id="7fb24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb24-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb24-109">Permission type</span></span>|<span data-ttu-id="7fb24-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fb24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb24-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fb24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fb24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7fb24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fb24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb24-114">Not supported.</span></span>|
|<span data-ttu-id="7fb24-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fb24-115">Application</span></span>|<span data-ttu-id="7fb24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb24-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fb24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fb24-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7fb24-118">Optional query parameters</span></span>
<span data-ttu-id="7fb24-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7fb24-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fb24-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fb24-120">Request headers</span></span>
|<span data-ttu-id="7fb24-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fb24-121">Header</span></span>|<span data-ttu-id="7fb24-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7fb24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb24-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fb24-123">Authorization</span></span>|<span data-ttu-id="7fb24-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fb24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fb24-125">Accept</span></span>|<span data-ttu-id="7fb24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb24-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fb24-127">Request body</span></span>
<span data-ttu-id="7fb24-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fb24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb24-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb24-129">Response</span></span>
<span data-ttu-id="7fb24-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7fb24-130">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb24-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7fb24-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb24-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fb24-132">Request</span></span>
<span data-ttu-id="7fb24-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb24-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="7fb24-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fb24-134">Response</span></span>
<span data-ttu-id="7fb24-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fb24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```



