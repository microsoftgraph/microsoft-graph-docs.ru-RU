---
title: Перечисление объектов webApp
description: Список свойств и связей объектов webApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fd4bee09a7e39179ed4d0c6ed25a40af0e4c927c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394721"
---
# <a name="list-webapps"></a><span data-ttu-id="d7eb8-103">Перечисление объектов webApp</span><span class="sxs-lookup"><span data-stu-id="d7eb8-103">List webApps</span></span>

> <span data-ttu-id="d7eb8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7eb8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7eb8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7eb8-107">Список свойств и связей объектов [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7eb8-107">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7eb8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7eb8-108">Prerequisites</span></span>
<span data-ttu-id="d7eb8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7eb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7eb8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7eb8-111">Permission type</span></span>|<span data-ttu-id="d7eb8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7eb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7eb8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7eb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7eb8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7eb8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d7eb8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7eb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7eb8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-116">Not supported.</span></span>|
|<span data-ttu-id="d7eb8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7eb8-117">Application</span></span>|<span data-ttu-id="d7eb8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7eb8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7eb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d7eb8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7eb8-120">Request headers</span></span>
|<span data-ttu-id="d7eb8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7eb8-121">Header</span></span>|<span data-ttu-id="d7eb8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7eb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7eb8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7eb8-123">Authorization</span></span>|<span data-ttu-id="d7eb8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7eb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7eb8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7eb8-125">Accept</span></span>|<span data-ttu-id="d7eb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7eb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7eb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7eb8-127">Request body</span></span>
<span data-ttu-id="d7eb8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7eb8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7eb8-129">Response</span></span>
<span data-ttu-id="d7eb8-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [webApp](../resources/intune-apps-webapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-130">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7eb8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d7eb8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7eb8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7eb8-132">Request</span></span>
<span data-ttu-id="d7eb8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="d7eb8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7eb8-134">Response</span></span>
<span data-ttu-id="d7eb8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7eb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1061

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```




