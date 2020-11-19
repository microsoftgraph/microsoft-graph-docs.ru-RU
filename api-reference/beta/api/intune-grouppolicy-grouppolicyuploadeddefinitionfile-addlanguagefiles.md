---
title: действие Аддлангуажефилес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e13619447a41b3c689fba5759fa6fa4bb43bfb1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224951"
---
# <a name="addlanguagefiles-action"></a><span data-ttu-id="bf793-103">действие Аддлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="bf793-103">addLanguageFiles action</span></span>

<span data-ttu-id="bf793-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf793-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf793-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf793-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf793-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf793-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf793-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf793-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf793-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf793-108">Prerequisites</span></span>
<span data-ttu-id="bf793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf793-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf793-111">Permission type</span></span>|<span data-ttu-id="bf793-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf793-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf793-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf793-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf793-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf793-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf793-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf793-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf793-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf793-116">Not supported.</span></span>|
|<span data-ttu-id="bf793-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf793-117">Application</span></span>|<span data-ttu-id="bf793-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf793-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf793-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf793-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/addLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="bf793-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf793-120">Request headers</span></span>
|<span data-ttu-id="bf793-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf793-121">Header</span></span>|<span data-ttu-id="bf793-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf793-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf793-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf793-123">Authorization</span></span>|<span data-ttu-id="bf793-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf793-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf793-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf793-125">Accept</span></span>|<span data-ttu-id="bf793-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf793-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf793-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf793-127">Request body</span></span>
<span data-ttu-id="bf793-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf793-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bf793-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="bf793-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bf793-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf793-130">Property</span></span>|<span data-ttu-id="bf793-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf793-131">Type</span></span>|<span data-ttu-id="bf793-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf793-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf793-133">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="bf793-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="bf793-134">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="bf793-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="bf793-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf793-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf793-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf793-136">Response</span></span>
<span data-ttu-id="bf793-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf793-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf793-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bf793-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf793-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf793-139">Request</span></span>
<span data-ttu-id="bf793-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf793-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/addLanguageFiles

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

### <a name="response"></a><span data-ttu-id="bf793-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf793-141">Response</span></span>
<span data-ttu-id="bf793-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




