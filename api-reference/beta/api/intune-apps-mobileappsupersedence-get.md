---
title: Получение Мобилеаппсуперседенце
description: Чтение свойств и связей объекта Мобилеаппсуперседенце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 370400312863274c21e97d32c7f58cce4b5f6018
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247953"
---
# <a name="get-mobileappsupersedence"></a><span data-ttu-id="953db-103">Получение Мобилеаппсуперседенце</span><span class="sxs-lookup"><span data-stu-id="953db-103">Get mobileAppSupersedence</span></span>

<span data-ttu-id="953db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="953db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="953db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="953db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="953db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="953db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="953db-107">Чтение свойств и связей объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="953db-107">Read properties and relationships of the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="953db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="953db-108">Prerequisites</span></span>
<span data-ttu-id="953db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="953db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="953db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="953db-111">Permission type</span></span>|<span data-ttu-id="953db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="953db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="953db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="953db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="953db-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="953db-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="953db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="953db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="953db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="953db-116">Not supported.</span></span>|
|<span data-ttu-id="953db-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="953db-117">Application</span></span>|<span data-ttu-id="953db-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="953db-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="953db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="953db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="953db-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="953db-120">Optional query parameters</span></span>
<span data-ttu-id="953db-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="953db-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="953db-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="953db-122">Request headers</span></span>
|<span data-ttu-id="953db-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="953db-123">Header</span></span>|<span data-ttu-id="953db-124">Значение</span><span class="sxs-lookup"><span data-stu-id="953db-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="953db-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="953db-125">Authorization</span></span>|<span data-ttu-id="953db-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="953db-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="953db-127">Accept</span><span class="sxs-lookup"><span data-stu-id="953db-127">Accept</span></span>|<span data-ttu-id="953db-128">application/json</span><span class="sxs-lookup"><span data-stu-id="953db-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="953db-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="953db-129">Request body</span></span>
<span data-ttu-id="953db-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="953db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="953db-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="953db-131">Response</span></span>
<span data-ttu-id="953db-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="953db-132">If successful, this method returns a `200 OK` response code and [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="953db-133">Пример</span><span class="sxs-lookup"><span data-stu-id="953db-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="953db-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="953db-134">Request</span></span>
<span data-ttu-id="953db-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="953db-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="953db-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="953db-136">Response</span></span>
<span data-ttu-id="953db-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="953db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppSupersedence",
    "id": "c0254204-4204-c025-0442-25c0044225c0",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "targetDisplayVersion": "Target Display Version value",
    "targetPublisher": "Target Publisher value",
    "targetType": "parent",
    "supersedenceType": "replace",
    "supersededAppCount": 2,
    "supersedingAppCount": 3
  }
}
```




