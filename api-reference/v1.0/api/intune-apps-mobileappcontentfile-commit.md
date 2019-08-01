---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02f7c4841af3e335a5935c604e6cfdfdfac52309
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016050"
---
# <a name="commit-action"></a><span data-ttu-id="22c61-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="22c61-103">commit action</span></span>

> <span data-ttu-id="22c61-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22c61-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22c61-105">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="22c61-105">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22c61-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="22c61-106">Prerequisites</span></span>
<span data-ttu-id="22c61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22c61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22c61-109">Permission type</span></span>|<span data-ttu-id="22c61-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22c61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22c61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22c61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22c61-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22c61-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22c61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22c61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22c61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22c61-114">Not supported.</span></span>|
|<span data-ttu-id="22c61-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22c61-115">Application</span></span>|<span data-ttu-id="22c61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22c61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22c61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22c61-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="22c61-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22c61-118">Request headers</span></span>
|<span data-ttu-id="22c61-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22c61-119">Header</span></span>|<span data-ttu-id="22c61-120">Значение</span><span class="sxs-lookup"><span data-stu-id="22c61-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22c61-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22c61-121">Authorization</span></span>|<span data-ttu-id="22c61-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22c61-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22c61-123">Accept</span><span class="sxs-lookup"><span data-stu-id="22c61-123">Accept</span></span>|<span data-ttu-id="22c61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22c61-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22c61-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22c61-125">Request body</span></span>
<span data-ttu-id="22c61-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22c61-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="22c61-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="22c61-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="22c61-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="22c61-128">Property</span></span>|<span data-ttu-id="22c61-129">Тип</span><span class="sxs-lookup"><span data-stu-id="22c61-129">Type</span></span>|<span data-ttu-id="22c61-130">Описание</span><span class="sxs-lookup"><span data-stu-id="22c61-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22c61-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="22c61-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="22c61-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="22c61-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="22c61-133">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="22c61-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="22c61-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="22c61-134">Response</span></span>
<span data-ttu-id="22c61-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22c61-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22c61-136">Пример</span><span class="sxs-lookup"><span data-stu-id="22c61-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="22c61-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="22c61-137">Request</span></span>
<span data-ttu-id="22c61-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22c61-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="22c61-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="22c61-139">Response</span></span>
<span data-ttu-id="22c61-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22c61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



