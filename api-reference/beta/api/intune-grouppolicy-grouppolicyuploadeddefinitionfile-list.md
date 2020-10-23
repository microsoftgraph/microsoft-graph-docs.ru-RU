---
title: Список Граупполициуплоадеддефинитионфилес
description: Список свойств и связей объектов Граупполициуплоадеддефинитионфиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa42ece9941ea8a3d235d56fe8f23d72ba3342df
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726628"
---
# <a name="list-grouppolicyuploadeddefinitionfiles"></a><span data-ttu-id="33bbd-103">Список Граупполициуплоадеддефинитионфилес</span><span class="sxs-lookup"><span data-stu-id="33bbd-103">List groupPolicyUploadedDefinitionFiles</span></span>

<span data-ttu-id="33bbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33bbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33bbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33bbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33bbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33bbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33bbd-107">Список свойств и связей объектов [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="33bbd-107">List properties and relationships of the [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33bbd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33bbd-108">Prerequisites</span></span>
<span data-ttu-id="33bbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33bbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33bbd-111">Permission type</span></span>|<span data-ttu-id="33bbd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33bbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33bbd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33bbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33bbd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33bbd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33bbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33bbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33bbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33bbd-116">Not supported.</span></span>|
|<span data-ttu-id="33bbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33bbd-117">Application</span></span>|<span data-ttu-id="33bbd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33bbd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33bbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33bbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="33bbd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33bbd-120">Request headers</span></span>
|<span data-ttu-id="33bbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33bbd-121">Header</span></span>|<span data-ttu-id="33bbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33bbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33bbd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33bbd-123">Authorization</span></span>|<span data-ttu-id="33bbd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33bbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33bbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33bbd-125">Accept</span></span>|<span data-ttu-id="33bbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33bbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33bbd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33bbd-127">Request body</span></span>
<span data-ttu-id="33bbd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33bbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33bbd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="33bbd-129">Response</span></span>
<span data-ttu-id="33bbd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33bbd-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33bbd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="33bbd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33bbd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33bbd-132">Request</span></span>
<span data-ttu-id="33bbd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33bbd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
```

### <a name="response"></a><span data-ttu-id="33bbd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33bbd-134">Response</span></span>
<span data-ttu-id="33bbd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33bbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1176

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
      "displayName": "Display Name value",
      "description": "Description value",
      "languageCodes": [
        "Language Codes value"
      ],
      "targetPrefix": "Target Prefix value",
      "targetNamespace": "Target Namespace value",
      "policyType": "admxIngested",
      "revision": "Revision value",
      "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "fileName": "File Name value",
      "status": "uploadInProgress",
      "content": "Y29udGVudA==",
      "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
      "defaultLanguageCode": "Default Language Code value",
      "groupPolicyUploadedLanguageFiles": [
        {
          "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
          "fileName": "File Name value",
          "languageCode": "Language Code value",
          "content": "Y29udGVudA==",
          "id": "Id value",
          "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
        }
      ]
    }
  ]
}
```





