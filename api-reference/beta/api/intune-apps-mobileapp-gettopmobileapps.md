---
title: Функция getTopMobileApps
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56d1fc98281591fdf331992ddd7b3a5f23053234
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961051"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="98238-103">Функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="98238-103">getTopMobileApps function</span></span>

> <span data-ttu-id="98238-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98238-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98238-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98238-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98238-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98238-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98238-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98238-107">Prerequisites</span></span>
<span data-ttu-id="98238-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98238-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98238-110">Permission type</span></span>|<span data-ttu-id="98238-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98238-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98238-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98238-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98238-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="98238-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="98238-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98238-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98238-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98238-115">Not supported.</span></span>|
|<span data-ttu-id="98238-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98238-116">Application</span></span>|<span data-ttu-id="98238-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98238-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98238-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98238-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="98238-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98238-119">Request headers</span></span>
|<span data-ttu-id="98238-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98238-120">Header</span></span>|<span data-ttu-id="98238-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98238-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98238-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98238-122">Authorization</span></span>|<span data-ttu-id="98238-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98238-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98238-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98238-124">Accept</span></span>|<span data-ttu-id="98238-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98238-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98238-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98238-126">Request body</span></span>
<span data-ttu-id="98238-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="98238-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="98238-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="98238-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="98238-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="98238-129">Property</span></span>|<span data-ttu-id="98238-130">Тип</span><span class="sxs-lookup"><span data-stu-id="98238-130">Type</span></span>|<span data-ttu-id="98238-131">Описание</span><span class="sxs-lookup"><span data-stu-id="98238-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98238-132">status</span><span class="sxs-lookup"><span data-stu-id="98238-132">status</span></span>|<span data-ttu-id="98238-133">String</span><span class="sxs-lookup"><span data-stu-id="98238-133">String</span></span>|<span data-ttu-id="98238-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98238-134">Not yet documented</span></span>|
|<span data-ttu-id="98238-135">count</span><span class="sxs-lookup"><span data-stu-id="98238-135">count</span></span>|<span data-ttu-id="98238-136">Int64</span><span class="sxs-lookup"><span data-stu-id="98238-136">Int64</span></span>|<span data-ttu-id="98238-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98238-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="98238-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="98238-138">Response</span></span>
<span data-ttu-id="98238-139">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [mobileApp](../resources/intune-apps-mobileapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98238-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98238-140">Пример</span><span class="sxs-lookup"><span data-stu-id="98238-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="98238-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="98238-141">Request</span></span>
<span data-ttu-id="98238-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98238-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="98238-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="98238-143">Response</span></span>
<span data-ttu-id="98238-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98238-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "dependentAppCount": 1
    }
  ]
}
```





