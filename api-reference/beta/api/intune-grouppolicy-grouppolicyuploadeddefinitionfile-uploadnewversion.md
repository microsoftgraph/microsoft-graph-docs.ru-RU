---
title: uploadNewVersion action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 803544b927623447ac2a148188563e87159de1b4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145602"
---
# <a name="uploadnewversion-action"></a><span data-ttu-id="aedc5-103">uploadNewVersion action</span><span class="sxs-lookup"><span data-stu-id="aedc5-103">uploadNewVersion action</span></span>

<span data-ttu-id="aedc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aedc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aedc5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aedc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aedc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aedc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aedc5-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aedc5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aedc5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aedc5-108">Prerequisites</span></span>
<span data-ttu-id="aedc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aedc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aedc5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aedc5-111">Permission type</span></span>|<span data-ttu-id="aedc5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aedc5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aedc5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aedc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aedc5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aedc5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aedc5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aedc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aedc5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aedc5-116">Not supported.</span></span>|
|<span data-ttu-id="aedc5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aedc5-117">Application</span></span>|<span data-ttu-id="aedc5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aedc5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aedc5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aedc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/uploadNewVersion
```

## <a name="request-headers"></a><span data-ttu-id="aedc5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aedc5-120">Request headers</span></span>
|<span data-ttu-id="aedc5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aedc5-121">Header</span></span>|<span data-ttu-id="aedc5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aedc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aedc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aedc5-123">Authorization</span></span>|<span data-ttu-id="aedc5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aedc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aedc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aedc5-125">Accept</span></span>|<span data-ttu-id="aedc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aedc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aedc5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aedc5-127">Request body</span></span>
<span data-ttu-id="aedc5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aedc5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aedc5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aedc5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aedc5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aedc5-130">Property</span></span>|<span data-ttu-id="aedc5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aedc5-131">Type</span></span>|<span data-ttu-id="aedc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aedc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aedc5-133">content</span><span class="sxs-lookup"><span data-stu-id="aedc5-133">content</span></span>|<span data-ttu-id="aedc5-134">Binary</span><span class="sxs-lookup"><span data-stu-id="aedc5-134">Binary</span></span>|<span data-ttu-id="aedc5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aedc5-135">Not yet documented</span></span>|
|<span data-ttu-id="aedc5-136">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="aedc5-136">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="aedc5-137">[коллекция groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="aedc5-137">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="aedc5-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aedc5-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aedc5-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="aedc5-139">Response</span></span>
<span data-ttu-id="aedc5-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aedc5-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aedc5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="aedc5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="aedc5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="aedc5-142">Request</span></span>
<span data-ttu-id="aedc5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aedc5-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/uploadNewVersion

Content-type: application/json
Content-length: 377

{
  "content": "Y29udGVudA==",
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
```

### <a name="response"></a><span data-ttu-id="aedc5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="aedc5-144">Response</span></span>
<span data-ttu-id="aedc5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aedc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




