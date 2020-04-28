---
title: Перечисление объектов iosVppEBook
description: Список свойств и связей объектов iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3a4010f9707294ff36f681fe7f65557d9f1e7c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392737"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="f4864-103">Перечисление объектов iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="f4864-103">List iosVppEBooks</span></span>

<span data-ttu-id="f4864-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4864-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4864-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4864-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4864-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4864-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4864-107">Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="f4864-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4864-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4864-108">Prerequisites</span></span>
<span data-ttu-id="f4864-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4864-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4864-111">Permission type</span></span>|<span data-ttu-id="f4864-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4864-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4864-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4864-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4864-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4864-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4864-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4864-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4864-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4864-116">Not supported.</span></span>|
|<span data-ttu-id="f4864-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4864-117">Application</span></span>|<span data-ttu-id="f4864-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4864-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4864-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4864-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="f4864-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4864-120">Request headers</span></span>
|<span data-ttu-id="f4864-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4864-121">Header</span></span>|<span data-ttu-id="f4864-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4864-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4864-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4864-123">Authorization</span></span>|<span data-ttu-id="f4864-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4864-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4864-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4864-125">Accept</span></span>|<span data-ttu-id="f4864-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4864-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4864-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4864-127">Request body</span></span>
<span data-ttu-id="f4864-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4864-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4864-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4864-129">Response</span></span>
<span data-ttu-id="f4864-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBook](../resources/intune-books-iosvppebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4864-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4864-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4864-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4864-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4864-132">Request</span></span>
<span data-ttu-id="f4864-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4864-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="f4864-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4864-134">Response</span></span>
<span data-ttu-id="f4864-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4864-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



