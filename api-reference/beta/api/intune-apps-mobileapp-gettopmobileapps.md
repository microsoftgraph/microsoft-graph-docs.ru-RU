---
title: функция getTopMobileApps
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d4f9299e2de7dca455d192637eba84ccc553d434
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879501"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="2da0f-103">функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="2da0f-103">getTopMobileApps function</span></span>

> <span data-ttu-id="2da0f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2da0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2da0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2da0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2da0f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2da0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2da0f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2da0f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2da0f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2da0f-108">Prerequisites</span></span>
<span data-ttu-id="2da0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2da0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2da0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2da0f-111">Permission type</span></span>|<span data-ttu-id="2da0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2da0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2da0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2da0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2da0f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2da0f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2da0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2da0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2da0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2da0f-116">Not supported.</span></span>|
|<span data-ttu-id="2da0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2da0f-117">Application</span></span>|<span data-ttu-id="2da0f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2da0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2da0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2da0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2da0f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2da0f-120">Request headers</span></span>
|<span data-ttu-id="2da0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2da0f-121">Header</span></span>|<span data-ttu-id="2da0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2da0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2da0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da0f-123">Authorization</span></span>|<span data-ttu-id="2da0f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2da0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2da0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2da0f-125">Accept</span></span>|<span data-ttu-id="2da0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2da0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2da0f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2da0f-127">Request body</span></span>
<span data-ttu-id="2da0f-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="2da0f-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2da0f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="2da0f-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2da0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2da0f-130">Property</span></span>|<span data-ttu-id="2da0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2da0f-131">Type</span></span>|<span data-ttu-id="2da0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2da0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2da0f-133">status</span><span class="sxs-lookup"><span data-stu-id="2da0f-133">status</span></span>|<span data-ttu-id="2da0f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2da0f-134">String</span></span>|<span data-ttu-id="2da0f-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2da0f-135">Not yet documented</span></span>|
|<span data-ttu-id="2da0f-136">count</span><span class="sxs-lookup"><span data-stu-id="2da0f-136">count</span></span>|<span data-ttu-id="2da0f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2da0f-137">Int64</span></span>|<span data-ttu-id="2da0f-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2da0f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2da0f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2da0f-139">Response</span></span>
<span data-ttu-id="2da0f-140">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [mobileApp](../resources/intune-apps-mobileapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2da0f-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da0f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2da0f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="2da0f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2da0f-142">Request</span></span>
<span data-ttu-id="2da0f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2da0f-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="2da0f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="2da0f-144">Response</span></span>
<span data-ttu-id="2da0f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

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
      "publishingState": "processing"
    }
  ]
}
```





