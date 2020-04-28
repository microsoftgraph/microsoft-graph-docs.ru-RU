---
title: действие Уплоадневверсион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e4cb80e314499b6f763a13fcb299daab863705a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391796"
---
# <a name="uploadnewversion-action"></a><span data-ttu-id="2fcbf-103">действие Уплоадневверсион</span><span class="sxs-lookup"><span data-stu-id="2fcbf-103">uploadNewVersion action</span></span>

<span data-ttu-id="2fcbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fcbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fcbf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fcbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fcbf-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fcbf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2fcbf-108">Prerequisites</span></span>
<span data-ttu-id="2fcbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fcbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fcbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fcbf-111">Permission type</span></span>|<span data-ttu-id="2fcbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fcbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fcbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fcbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fcbf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fcbf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fcbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fcbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fcbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-116">Not supported.</span></span>|
|<span data-ttu-id="2fcbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fcbf-117">Application</span></span>|<span data-ttu-id="2fcbf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fcbf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fcbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fcbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/uploadNewVersion
```

## <a name="request-headers"></a><span data-ttu-id="2fcbf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2fcbf-120">Request headers</span></span>
|<span data-ttu-id="2fcbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fcbf-121">Header</span></span>|<span data-ttu-id="2fcbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2fcbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fcbf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fcbf-123">Authorization</span></span>|<span data-ttu-id="2fcbf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fcbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fcbf-125">Accept</span></span>|<span data-ttu-id="2fcbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fcbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fcbf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2fcbf-127">Request body</span></span>
<span data-ttu-id="2fcbf-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2fcbf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2fcbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fcbf-130">Property</span></span>|<span data-ttu-id="2fcbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2fcbf-131">Type</span></span>|<span data-ttu-id="2fcbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2fcbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fcbf-133">content</span><span class="sxs-lookup"><span data-stu-id="2fcbf-133">content</span></span>|<span data-ttu-id="2fcbf-134">Binary</span><span class="sxs-lookup"><span data-stu-id="2fcbf-134">Binary</span></span>|<span data-ttu-id="2fcbf-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-135">Not yet documented</span></span>|
|<span data-ttu-id="2fcbf-136">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="2fcbf-136">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="2fcbf-137">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="2fcbf-137">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="2fcbf-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2fcbf-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fcbf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fcbf-139">Response</span></span>
<span data-ttu-id="2fcbf-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2fcbf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2fcbf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fcbf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fcbf-142">Request</span></span>
<span data-ttu-id="2fcbf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fcbf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fcbf-144">Response</span></span>
<span data-ttu-id="2fcbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fcbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



