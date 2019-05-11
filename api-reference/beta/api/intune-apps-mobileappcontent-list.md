---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6985c4996e88079b287d6ad0c8e4fe8aae41601c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935218"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="d4c14-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4c14-103">List mobileAppContents</span></span>

> <span data-ttu-id="d4c14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4c14-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4c14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c14-106">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4c14-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4c14-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d4c14-107">Prerequisites</span></span>
<span data-ttu-id="d4c14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c14-110">Permission type</span></span>|<span data-ttu-id="d4c14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4c14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4c14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4c14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d4c14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4c14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c14-115">Not supported.</span></span>|
|<span data-ttu-id="d4c14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4c14-116">Application</span></span>|<span data-ttu-id="d4c14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4c14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="d4c14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4c14-119">Request headers</span></span>
|<span data-ttu-id="d4c14-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4c14-120">Header</span></span>|<span data-ttu-id="d4c14-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d4c14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4c14-122">Authorization</span></span>|<span data-ttu-id="d4c14-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4c14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c14-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d4c14-124">Accept</span></span>|<span data-ttu-id="d4c14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c14-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4c14-126">Request body</span></span>
<span data-ttu-id="d4c14-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4c14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c14-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4c14-128">Response</span></span>
<span data-ttu-id="d4c14-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4c14-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c14-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d4c14-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4c14-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4c14-131">Request</span></span>
<span data-ttu-id="d4c14-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4c14-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="d4c14-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c14-133">Response</span></span>
<span data-ttu-id="d4c14-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4c14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```




