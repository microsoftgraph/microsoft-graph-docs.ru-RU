---
title: Get mobileAppDependency
description: Чтение свойств и связей объекта mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1256ea858627ca808446c389b08c9b8ed677b540
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155330"
---
# <a name="get-mobileappdependency"></a><span data-ttu-id="bc1f8-103">Get mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="bc1f8-103">Get mobileAppDependency</span></span>

<span data-ttu-id="bc1f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc1f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc1f8-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc1f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc1f8-107">Чтение свойств и связей объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="bc1f8-107">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc1f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc1f8-108">Prerequisites</span></span>
<span data-ttu-id="bc1f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc1f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc1f8-111">Permission type</span></span>|<span data-ttu-id="bc1f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc1f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc1f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc1f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc1f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc1f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bc1f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc1f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc1f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-116">Not supported.</span></span>|
|<span data-ttu-id="bc1f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc1f8-117">Application</span></span>|<span data-ttu-id="bc1f8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc1f8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc1f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc1f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc1f8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc1f8-120">Optional query parameters</span></span>
<span data-ttu-id="bc1f8-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc1f8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc1f8-122">Request headers</span></span>
|<span data-ttu-id="bc1f8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc1f8-123">Header</span></span>|<span data-ttu-id="bc1f8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bc1f8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc1f8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc1f8-125">Authorization</span></span>|<span data-ttu-id="bc1f8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc1f8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bc1f8-127">Accept</span></span>|<span data-ttu-id="bc1f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bc1f8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc1f8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc1f8-129">Request body</span></span>
<span data-ttu-id="bc1f8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc1f8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc1f8-131">Response</span></span>
<span data-ttu-id="bc1f8-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект mobileAppDependency](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-132">If successful, this method returns a `200 OK` response code and [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc1f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bc1f8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc1f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc1f8-134">Request</span></span>
<span data-ttu-id="bc1f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="bc1f8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc1f8-136">Response</span></span>
<span data-ttu-id="bc1f8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc1f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppDependency",
    "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "targetDisplayVersion": "Target Display Version value",
    "targetPublisher": "Target Publisher value",
    "targetType": "parent",
    "dependencyType": "autoInstall",
    "dependentAppCount": 1,
    "dependsOnAppCount": 1
  }
}
```




