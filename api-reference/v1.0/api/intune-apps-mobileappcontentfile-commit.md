---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d242d0bbf5fe69ae67167cb293582cbfc165220
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541705"
---
# <a name="commit-action"></a><span data-ttu-id="76bc6-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="76bc6-103">commit action</span></span>

> <span data-ttu-id="76bc6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76bc6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76bc6-105">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="76bc6-105">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76bc6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76bc6-106">Prerequisites</span></span>
<span data-ttu-id="76bc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76bc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76bc6-109">Permission type</span></span>|<span data-ttu-id="76bc6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76bc6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76bc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76bc6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76bc6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76bc6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76bc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76bc6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76bc6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76bc6-114">Not supported.</span></span>|
|<span data-ttu-id="76bc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76bc6-115">Application</span></span>|<span data-ttu-id="76bc6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76bc6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76bc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76bc6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="76bc6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76bc6-118">Request headers</span></span>
|<span data-ttu-id="76bc6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76bc6-119">Header</span></span>|<span data-ttu-id="76bc6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="76bc6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76bc6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76bc6-121">Authorization</span></span>|<span data-ttu-id="76bc6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76bc6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76bc6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="76bc6-123">Accept</span></span>|<span data-ttu-id="76bc6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76bc6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76bc6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76bc6-125">Request body</span></span>
<span data-ttu-id="76bc6-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76bc6-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="76bc6-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="76bc6-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="76bc6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="76bc6-128">Property</span></span>|<span data-ttu-id="76bc6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="76bc6-129">Type</span></span>|<span data-ttu-id="76bc6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="76bc6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76bc6-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="76bc6-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="76bc6-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="76bc6-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="76bc6-133">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="76bc6-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="76bc6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="76bc6-134">Response</span></span>
<span data-ttu-id="76bc6-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76bc6-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76bc6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="76bc6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="76bc6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="76bc6-137">Request</span></span>
<span data-ttu-id="76bc6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76bc6-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76bc6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="76bc6-139">Response</span></span>
<span data-ttu-id="76bc6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76bc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



