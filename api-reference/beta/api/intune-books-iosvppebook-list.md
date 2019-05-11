---
title: Перечисление объектов iosVppEBook
description: Список свойств и связей объектов iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 039c75d079aaadabfd802a1e78651b445d9bf155
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934294"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="73d06-103">Перечисление объектов iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="73d06-103">List iosVppEBooks</span></span>

> <span data-ttu-id="73d06-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73d06-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73d06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73d06-106">Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="73d06-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73d06-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="73d06-107">Prerequisites</span></span>
<span data-ttu-id="73d06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73d06-110">Permission type</span></span>|<span data-ttu-id="73d06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73d06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73d06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73d06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73d06-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73d06-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="73d06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73d06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d06-115">Not supported.</span></span>|
|<span data-ttu-id="73d06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73d06-116">Application</span></span>|<span data-ttu-id="73d06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73d06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73d06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="73d06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73d06-119">Request headers</span></span>
|<span data-ttu-id="73d06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73d06-120">Header</span></span>|<span data-ttu-id="73d06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73d06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73d06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73d06-122">Authorization</span></span>|<span data-ttu-id="73d06-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73d06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73d06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73d06-124">Accept</span></span>|<span data-ttu-id="73d06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73d06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d06-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73d06-126">Request body</span></span>
<span data-ttu-id="73d06-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73d06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d06-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="73d06-128">Response</span></span>
<span data-ttu-id="73d06-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBook](../resources/intune-books-iosvppebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73d06-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d06-130">Пример</span><span class="sxs-lookup"><span data-stu-id="73d06-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73d06-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="73d06-131">Request</span></span>
<span data-ttu-id="73d06-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73d06-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="73d06-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d06-133">Response</span></span>
<span data-ttu-id="73d06-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73d06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
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
  ]
}
```




