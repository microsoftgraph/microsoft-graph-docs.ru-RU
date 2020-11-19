---
title: действие Ремовелангуажефилес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30b1d7e06d69b768fd954a82b3ae3925cd274b42
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224713"
---
# <a name="removelanguagefiles-action"></a><span data-ttu-id="3f163-103">действие Ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="3f163-103">removeLanguageFiles action</span></span>

<span data-ttu-id="3f163-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f163-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f163-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f163-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f163-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f163-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f163-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f163-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f163-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3f163-108">Prerequisites</span></span>
<span data-ttu-id="3f163-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f163-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f163-111">Permission type</span></span>|<span data-ttu-id="3f163-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f163-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f163-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f163-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f163-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f163-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f163-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f163-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f163-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f163-116">Not supported.</span></span>|
|<span data-ttu-id="3f163-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f163-117">Application</span></span>|<span data-ttu-id="3f163-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f163-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f163-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f163-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/removeLanguageFiles
```

## <a name="request-headers"></a><span data-ttu-id="3f163-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f163-120">Request headers</span></span>
|<span data-ttu-id="3f163-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f163-121">Header</span></span>|<span data-ttu-id="3f163-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f163-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f163-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f163-123">Authorization</span></span>|<span data-ttu-id="3f163-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f163-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f163-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f163-125">Accept</span></span>|<span data-ttu-id="3f163-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f163-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f163-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f163-127">Request body</span></span>
<span data-ttu-id="3f163-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f163-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3f163-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3f163-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3f163-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f163-130">Property</span></span>|<span data-ttu-id="3f163-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f163-131">Type</span></span>|<span data-ttu-id="3f163-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f163-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f163-133">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="3f163-133">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="3f163-134">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="3f163-134">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="3f163-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3f163-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f163-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f163-136">Response</span></span>
<span data-ttu-id="3f163-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3f163-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f163-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3f163-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f163-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f163-139">Request</span></span>
<span data-ttu-id="3f163-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f163-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f163-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f163-141">Response</span></span>
<span data-ttu-id="3f163-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f163-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




