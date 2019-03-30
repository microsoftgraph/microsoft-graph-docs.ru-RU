---
title: Get macOSOfficeSuiteApp
description: Чтение свойств и связей объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6511aada777e7fcd6e4df7728b604cea49702e05
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987106"
---
# <a name="get-macosofficesuiteapp"></a><span data-ttu-id="70828-103">Get macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="70828-103">Get macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="70828-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70828-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70828-105">Чтение свойств и связей объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="70828-105">Read properties and relationships of the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70828-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="70828-106">Prerequisites</span></span>
<span data-ttu-id="70828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70828-109">Permission type</span></span>|<span data-ttu-id="70828-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70828-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70828-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70828-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70828-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70828-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70828-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70828-114">Not supported.</span></span>|
|<span data-ttu-id="70828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70828-115">Application</span></span>|<span data-ttu-id="70828-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70828-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70828-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70828-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70828-118">Optional query parameters</span></span>
<span data-ttu-id="70828-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70828-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70828-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70828-120">Request headers</span></span>
|<span data-ttu-id="70828-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70828-121">Header</span></span>|<span data-ttu-id="70828-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70828-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70828-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70828-123">Authorization</span></span>|<span data-ttu-id="70828-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70828-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70828-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70828-125">Accept</span></span>|<span data-ttu-id="70828-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70828-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70828-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70828-127">Request body</span></span>
<span data-ttu-id="70828-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70828-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70828-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="70828-129">Response</span></span>
<span data-ttu-id="70828-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="70828-130">If successful, this method returns a `200 OK` response code and [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70828-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70828-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="70828-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70828-132">Request</span></span>
<span data-ttu-id="70828-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70828-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="70828-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70828-134">Response</span></span>
<span data-ttu-id="70828-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70828-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
    "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing"
  }
}
```



