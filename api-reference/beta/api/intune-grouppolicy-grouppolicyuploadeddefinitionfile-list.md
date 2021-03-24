---
title: List groupPolicyUploadedDefinitionFiles
description: Список свойств и связей объектов groupPolicyUploadedDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 390d5ad0b879b8eeff7fd9b80ed4d851af5a2703
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145672"
---
# <a name="list-grouppolicyuploadeddefinitionfiles"></a><span data-ttu-id="58219-103">List groupPolicyUploadedDefinitionFiles</span><span class="sxs-lookup"><span data-stu-id="58219-103">List groupPolicyUploadedDefinitionFiles</span></span>

<span data-ttu-id="58219-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58219-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58219-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58219-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58219-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58219-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58219-107">Список свойств и связей [объектов groupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="58219-107">List properties and relationships of the [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58219-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58219-108">Prerequisites</span></span>
<span data-ttu-id="58219-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58219-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58219-111">Permission type</span></span>|<span data-ttu-id="58219-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58219-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58219-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58219-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58219-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58219-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58219-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58219-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58219-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58219-116">Not supported.</span></span>|
|<span data-ttu-id="58219-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58219-117">Application</span></span>|<span data-ttu-id="58219-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58219-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58219-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58219-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="58219-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58219-120">Request headers</span></span>
|<span data-ttu-id="58219-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58219-121">Header</span></span>|<span data-ttu-id="58219-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58219-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58219-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58219-123">Authorization</span></span>|<span data-ttu-id="58219-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58219-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58219-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58219-125">Accept</span></span>|<span data-ttu-id="58219-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58219-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58219-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58219-127">Request body</span></span>
<span data-ttu-id="58219-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58219-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58219-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="58219-129">Response</span></span>
<span data-ttu-id="58219-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="58219-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58219-131">Пример</span><span class="sxs-lookup"><span data-stu-id="58219-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="58219-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="58219-132">Request</span></span>
<span data-ttu-id="58219-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58219-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
```

### <a name="response"></a><span data-ttu-id="58219-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="58219-134">Response</span></span>
<span data-ttu-id="58219-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58219-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




