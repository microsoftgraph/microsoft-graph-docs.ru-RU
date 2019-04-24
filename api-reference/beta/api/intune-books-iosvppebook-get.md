---
title: Get iosVppEBook
description: Чтение свойств и связей объекта iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69b0bfc218c27d821b9d0842bfa92f16569488d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483700"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="3c447-103">Get iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="3c447-103">Get iosVppEBook</span></span>

> <span data-ttu-id="3c447-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c447-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c447-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c447-106">Чтение свойств и связей объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3c447-106">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c447-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3c447-107">Prerequisites</span></span>
<span data-ttu-id="3c447-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c447-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c447-110">Permission type</span></span>|<span data-ttu-id="3c447-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c447-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c447-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c447-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c447-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c447-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3c447-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c447-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c447-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c447-115">Not supported.</span></span>|
|<span data-ttu-id="3c447-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c447-116">Application</span></span>|<span data-ttu-id="3c447-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c447-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c447-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c447-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c447-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c447-119">Optional query parameters</span></span>
<span data-ttu-id="3c447-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c447-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c447-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c447-121">Request headers</span></span>
|<span data-ttu-id="3c447-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c447-122">Header</span></span>|<span data-ttu-id="3c447-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3c447-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c447-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c447-124">Authorization</span></span>|<span data-ttu-id="3c447-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c447-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c447-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3c447-126">Accept</span></span>|<span data-ttu-id="3c447-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3c447-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c447-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c447-128">Request body</span></span>
<span data-ttu-id="3c447-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c447-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c447-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c447-130">Response</span></span>
<span data-ttu-id="3c447-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c447-131">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c447-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3c447-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c447-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c447-133">Request</span></span>
<span data-ttu-id="3c447-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c447-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="3c447-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c447-135">Response</span></span>
<span data-ttu-id="3c447-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBook",
    "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
    "largeCover": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "informationUrl": "https://example.com/informationUrl/",
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
    "appleId": "Apple Id value",
    "vppOrganizationName": "Vpp Organization Name value",
    "genres": [
      "Genres value"
    ],
    "language": "Language value",
    "seller": "Seller value",
    "totalLicenseCount": 1,
    "usedLicenseCount": 0,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





