---
title: функция getTopMobileApps
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f29c6dfe6502b1520e2100781d47688bbbe5d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417030"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="ade29-103">функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="ade29-103">getTopMobileApps function</span></span>

> <span data-ttu-id="ade29-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ade29-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ade29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ade29-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ade29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ade29-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ade29-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ade29-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ade29-108">Prerequisites</span></span>
<span data-ttu-id="ade29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ade29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ade29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ade29-111">Permission type</span></span>|<span data-ttu-id="ade29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ade29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ade29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ade29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ade29-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ade29-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ade29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ade29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ade29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade29-116">Not supported.</span></span>|
|<span data-ttu-id="ade29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ade29-117">Application</span></span>|<span data-ttu-id="ade29-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ade29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ade29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ade29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ade29-120">Request headers</span></span>
|<span data-ttu-id="ade29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ade29-121">Header</span></span>|<span data-ttu-id="ade29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ade29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ade29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade29-123">Authorization</span></span>|<span data-ttu-id="ade29-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ade29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ade29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ade29-125">Accept</span></span>|<span data-ttu-id="ade29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ade29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ade29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ade29-127">Request body</span></span>
<span data-ttu-id="ade29-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ade29-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ade29-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ade29-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ade29-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ade29-130">Property</span></span>|<span data-ttu-id="ade29-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ade29-131">Type</span></span>|<span data-ttu-id="ade29-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ade29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ade29-133">status</span><span class="sxs-lookup"><span data-stu-id="ade29-133">status</span></span>|<span data-ttu-id="ade29-134">String</span><span class="sxs-lookup"><span data-stu-id="ade29-134">String</span></span>|<span data-ttu-id="ade29-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ade29-135">Not yet documented</span></span>|
|<span data-ttu-id="ade29-136">count</span><span class="sxs-lookup"><span data-stu-id="ade29-136">count</span></span>|<span data-ttu-id="ade29-137">Int64</span><span class="sxs-lookup"><span data-stu-id="ade29-137">Int64</span></span>|<span data-ttu-id="ade29-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ade29-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ade29-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ade29-139">Response</span></span>
<span data-ttu-id="ade29-140">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [mobileApp](../resources/intune-apps-mobileapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ade29-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade29-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ade29-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ade29-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ade29-142">Request</span></span>
<span data-ttu-id="ade29-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ade29-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="ade29-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ade29-144">Response</span></span>
<span data-ttu-id="ade29-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ade29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

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
      ]
    }
  ]
}
```




