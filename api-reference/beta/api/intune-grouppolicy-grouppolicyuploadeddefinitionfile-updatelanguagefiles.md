---
title: действие Упдателангуажефилес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 631a147bf095930f12b729ae0ab79e01f1bffa91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440892"
---
# <a name="updatelanguagefiles-action"></a><span data-ttu-id="a2892-103">действие Упдателангуажефилес</span><span class="sxs-lookup"><span data-stu-id="a2892-103">updateLanguageFiles action</span></span>

<span data-ttu-id="a2892-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2892-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2892-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2892-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2892-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2892-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2892-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a2892-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2892-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2892-108">Prerequisites</span></span>
<span data-ttu-id="a2892-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2892-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2892-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2892-111">Permission type</span></span>|<span data-ttu-id="a2892-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2892-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2892-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2892-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2892-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2892-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2892-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2892-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2892-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2892-116">Not supported.</span></span>|
|<span data-ttu-id="a2892-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2892-117">Application</span></span>|<span data-ttu-id="a2892-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2892-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2892-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2892-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/updateLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="a2892-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2892-120">Request headers</span></span>
|<span data-ttu-id="a2892-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2892-121">Header</span></span>|<span data-ttu-id="a2892-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2892-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2892-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2892-123">Authorization</span></span>|<span data-ttu-id="a2892-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2892-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2892-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2892-125">Accept</span></span>|<span data-ttu-id="a2892-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2892-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2892-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2892-127">Request body</span></span>
<span data-ttu-id="a2892-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2892-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a2892-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a2892-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a2892-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2892-130">Property</span></span>|<span data-ttu-id="a2892-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2892-131">Type</span></span>|<span data-ttu-id="a2892-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2892-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2892-133">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="a2892-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="a2892-134">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="a2892-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="a2892-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a2892-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2892-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2892-136">Response</span></span>
<span data-ttu-id="a2892-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2892-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2892-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a2892-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2892-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2892-139">Request</span></span>
<span data-ttu-id="a2892-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2892-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2892-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2892-141">Response</span></span>
<span data-ttu-id="a2892-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2892-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



