---
title: Получение Мобилеаппдепенденци
description: Чтение свойств и связей объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed575e48a2fb8d175d7d459c84a7fe9c6332c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935153"
---
# <a name="get-mobileappdependency"></a><span data-ttu-id="2ddaa-103">Получение Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="2ddaa-103">Get mobileAppDependency</span></span>

> <span data-ttu-id="2ddaa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ddaa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ddaa-106">Чтение свойств и связей объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="2ddaa-106">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ddaa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ddaa-107">Prerequisites</span></span>
<span data-ttu-id="2ddaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ddaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ddaa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ddaa-110">Permission type</span></span>|<span data-ttu-id="2ddaa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ddaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ddaa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ddaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ddaa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ddaa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ddaa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ddaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ddaa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-115">Not supported.</span></span>|
|<span data-ttu-id="2ddaa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ddaa-116">Application</span></span>|<span data-ttu-id="2ddaa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ddaa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ddaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ddaa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ddaa-119">Optional query parameters</span></span>
<span data-ttu-id="2ddaa-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ddaa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ddaa-121">Request headers</span></span>
|<span data-ttu-id="2ddaa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ddaa-122">Header</span></span>|<span data-ttu-id="2ddaa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2ddaa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ddaa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ddaa-124">Authorization</span></span>|<span data-ttu-id="2ddaa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ddaa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2ddaa-126">Accept</span></span>|<span data-ttu-id="2ddaa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2ddaa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ddaa-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ddaa-128">Request body</span></span>
<span data-ttu-id="2ddaa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ddaa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ddaa-130">Response</span></span>
<span data-ttu-id="2ddaa-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-131">If successful, this method returns a `200 OK` response code and [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ddaa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2ddaa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ddaa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ddaa-133">Request</span></span>
<span data-ttu-id="2ddaa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="2ddaa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ddaa-135">Response</span></span>
<span data-ttu-id="2ddaa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ddaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppDependency",
    "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "dependencyType": "autoInstall",
    "dependentAppCount": 1
  }
}
```




