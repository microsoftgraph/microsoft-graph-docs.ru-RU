---
title: updateLanguageFiles action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 900825b8db43fea285a8c54825e4a8e56570d06d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145609"
---
# <a name="updatelanguagefiles-action"></a><span data-ttu-id="0b500-103">updateLanguageFiles action</span><span class="sxs-lookup"><span data-stu-id="0b500-103">updateLanguageFiles action</span></span>

<span data-ttu-id="0b500-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b500-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b500-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b500-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b500-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b500-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b500-108">Prerequisites</span></span>
<span data-ttu-id="0b500-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b500-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b500-111">Permission type</span></span>|<span data-ttu-id="0b500-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b500-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b500-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b500-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b500-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b500-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b500-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b500-116">Not supported.</span></span>|
|<span data-ttu-id="0b500-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b500-117">Application</span></span>|<span data-ttu-id="0b500-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b500-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b500-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/updateLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="0b500-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b500-120">Request headers</span></span>
|<span data-ttu-id="0b500-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b500-121">Header</span></span>|<span data-ttu-id="0b500-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b500-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b500-123">Authorization</span></span>|<span data-ttu-id="0b500-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b500-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b500-125">Accept</span></span>|<span data-ttu-id="0b500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b500-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b500-127">Request body</span></span>
<span data-ttu-id="0b500-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b500-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b500-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0b500-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b500-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b500-130">Property</span></span>|<span data-ttu-id="0b500-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b500-131">Type</span></span>|<span data-ttu-id="0b500-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b500-133">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="0b500-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="0b500-134">[коллекция groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="0b500-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="0b500-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b500-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0b500-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b500-136">Response</span></span>
<span data-ttu-id="0b500-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b500-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b500-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0b500-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b500-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b500-139">Request</span></span>
<span data-ttu-id="0b500-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b500-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/updateLanguageFiles

Content-type: application/json
Content-length: 347

{
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

### <a name="response"></a><span data-ttu-id="0b500-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b500-141">Response</span></span>
<span data-ttu-id="0b500-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b500-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




