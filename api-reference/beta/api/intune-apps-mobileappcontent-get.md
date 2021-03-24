---
title: Get mobileAppContent
description: Чтение свойств и связей объекта mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afd0e90702fe80f716f93bb2e8a1f2130a9f7b48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139841"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="e7431-103">Get mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e7431-103">Get mobileAppContent</span></span>

<span data-ttu-id="e7431-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7431-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7431-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7431-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7431-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7431-107">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e7431-107">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7431-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e7431-108">Prerequisites</span></span>
<span data-ttu-id="e7431-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7431-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7431-111">Permission type</span></span>|<span data-ttu-id="e7431-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7431-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7431-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7431-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7431-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7431-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7431-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7431-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7431-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7431-116">Not supported.</span></span>|
|<span data-ttu-id="e7431-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e7431-117">Application</span></span>|<span data-ttu-id="e7431-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7431-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7431-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7431-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7431-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e7431-120">Optional query parameters</span></span>
<span data-ttu-id="e7431-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e7431-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7431-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7431-122">Request headers</span></span>
|<span data-ttu-id="e7431-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7431-123">Header</span></span>|<span data-ttu-id="e7431-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e7431-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7431-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7431-125">Authorization</span></span>|<span data-ttu-id="e7431-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7431-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7431-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e7431-127">Accept</span></span>|<span data-ttu-id="e7431-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7431-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7431-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7431-129">Request body</span></span>
<span data-ttu-id="e7431-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7431-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7431-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7431-131">Response</span></span>
<span data-ttu-id="e7431-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e7431-132">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7431-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e7431-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7431-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7431-134">Request</span></span>
<span data-ttu-id="e7431-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7431-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="e7431-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7431-136">Response</span></span>
<span data-ttu-id="e7431-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




