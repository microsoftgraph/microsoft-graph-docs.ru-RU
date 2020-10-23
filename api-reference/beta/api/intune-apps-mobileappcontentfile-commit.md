---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0517047b0a3c7d1e8f31aeb8a457691e2d23c5e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695966"
---
# <a name="commit-action"></a><span data-ttu-id="c7947-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="c7947-103">commit action</span></span>

<span data-ttu-id="c7947-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7947-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7947-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7947-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7947-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7947-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7947-107">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="c7947-107">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7947-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7947-108">Prerequisites</span></span>
<span data-ttu-id="c7947-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7947-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7947-111">Permission type</span></span>|<span data-ttu-id="c7947-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7947-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7947-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7947-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7947-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7947-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7947-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7947-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7947-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7947-116">Not supported.</span></span>|
|<span data-ttu-id="c7947-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7947-117">Application</span></span>|<span data-ttu-id="c7947-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7947-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7947-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7947-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="c7947-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7947-120">Request headers</span></span>
|<span data-ttu-id="c7947-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7947-121">Header</span></span>|<span data-ttu-id="c7947-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7947-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7947-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7947-123">Authorization</span></span>|<span data-ttu-id="c7947-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7947-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7947-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7947-125">Accept</span></span>|<span data-ttu-id="c7947-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7947-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7947-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7947-127">Request body</span></span>
<span data-ttu-id="c7947-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7947-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7947-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c7947-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7947-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7947-130">Property</span></span>|<span data-ttu-id="c7947-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7947-131">Type</span></span>|<span data-ttu-id="c7947-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7947-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7947-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="c7947-133">fileEncryptionInfo</span></span>|[<span data-ttu-id="c7947-134">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="c7947-134">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="c7947-135">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="c7947-135">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="c7947-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7947-136">Response</span></span>
<span data-ttu-id="c7947-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7947-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7947-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c7947-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7947-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7947-139">Request</span></span>
<span data-ttu-id="c7947-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7947-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

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

### <a name="response"></a><span data-ttu-id="c7947-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7947-141">Response</span></span>
<span data-ttu-id="c7947-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7947-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





