---
title: Получение Микрософтсторефорбусинессконтаинедапп
description: Чтение свойств и связей объекта Микрософтсторефорбусинессконтаинедапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e19bd01922e2aa23a92759ff67ff2680d9ad05eb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761449"
---
# <a name="get-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="9da82-103">Получение Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="9da82-103">Get microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="9da82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9da82-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9da82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9da82-106">Чтение свойств и связей объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9da82-106">Read properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9da82-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9da82-107">Prerequisites</span></span>
<span data-ttu-id="9da82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9da82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9da82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9da82-110">Permission type</span></span>|<span data-ttu-id="9da82-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9da82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9da82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9da82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9da82-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9da82-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9da82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9da82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9da82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da82-115">Not supported.</span></span>|
|<span data-ttu-id="9da82-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9da82-116">Application</span></span>|<span data-ttu-id="9da82-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9da82-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9da82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9da82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9da82-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9da82-119">Optional query parameters</span></span>
<span data-ttu-id="9da82-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9da82-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9da82-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9da82-121">Request headers</span></span>
|<span data-ttu-id="9da82-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9da82-122">Header</span></span>|<span data-ttu-id="9da82-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9da82-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9da82-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9da82-124">Authorization</span></span>|<span data-ttu-id="9da82-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9da82-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9da82-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9da82-126">Accept</span></span>|<span data-ttu-id="9da82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9da82-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9da82-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9da82-128">Request body</span></span>
<span data-ttu-id="9da82-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9da82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9da82-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9da82-130">Response</span></span>
<span data-ttu-id="9da82-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9da82-131">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9da82-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9da82-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9da82-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9da82-133">Request</span></span>
<span data-ttu-id="9da82-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9da82-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="9da82-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9da82-135">Response</span></span>
<span data-ttu-id="9da82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9da82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
    "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
    "appUserModelId": "App User Model Id value"
  }
}
```




