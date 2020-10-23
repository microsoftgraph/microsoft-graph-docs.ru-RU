---
title: действие Ремовелангуажефилес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1d8945d36c5860695019c203869da0fd09b0043
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726614"
---
# <a name="removelanguagefiles-action"></a><span data-ttu-id="7f046-103">действие Ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="7f046-103">removeLanguageFiles action</span></span>

<span data-ttu-id="7f046-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f046-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f046-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f046-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f046-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f046-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f046-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f046-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f046-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f046-108">Prerequisites</span></span>
<span data-ttu-id="7f046-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f046-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f046-111">Permission type</span></span>|<span data-ttu-id="7f046-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f046-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f046-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f046-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f046-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f046-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f046-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f046-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f046-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f046-116">Not supported.</span></span>|
|<span data-ttu-id="7f046-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f046-117">Application</span></span>|<span data-ttu-id="7f046-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f046-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f046-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f046-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="7f046-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f046-120">Request headers</span></span>
|<span data-ttu-id="7f046-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f046-121">Header</span></span>|<span data-ttu-id="7f046-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f046-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f046-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f046-123">Authorization</span></span>|<span data-ttu-id="7f046-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f046-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f046-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f046-125">Accept</span></span>|<span data-ttu-id="7f046-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f046-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f046-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f046-127">Request body</span></span>
<span data-ttu-id="7f046-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f046-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7f046-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7f046-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7f046-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f046-130">Property</span></span>|<span data-ttu-id="7f046-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f046-131">Type</span></span>|<span data-ttu-id="7f046-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f046-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f046-133">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="7f046-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="7f046-134">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="7f046-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="7f046-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f046-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7f046-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f046-136">Response</span></span>
<span data-ttu-id="7f046-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f046-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f046-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7f046-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f046-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f046-139">Request</span></span>
<span data-ttu-id="7f046-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f046-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles

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

### <a name="response"></a><span data-ttu-id="7f046-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f046-141">Response</span></span>
<span data-ttu-id="7f046-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f046-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





