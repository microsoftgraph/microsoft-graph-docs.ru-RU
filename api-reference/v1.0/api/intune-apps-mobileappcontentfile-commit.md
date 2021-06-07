---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc2f4a3db1b53958a5055a302f9e4db57e19e91e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754072"
---
# <a name="commit-action"></a><span data-ttu-id="75fe6-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="75fe6-103">commit action</span></span>

<span data-ttu-id="75fe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75fe6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75fe6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75fe6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75fe6-106">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="75fe6-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75fe6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75fe6-107">Prerequisites</span></span>
<span data-ttu-id="75fe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75fe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75fe6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75fe6-110">Permission type</span></span>|<span data-ttu-id="75fe6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75fe6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75fe6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75fe6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75fe6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fe6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75fe6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75fe6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75fe6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fe6-115">Not supported.</span></span>|
|<span data-ttu-id="75fe6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="75fe6-116">Application</span></span>|<span data-ttu-id="75fe6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fe6-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75fe6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75fe6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="75fe6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75fe6-119">Request headers</span></span>
|<span data-ttu-id="75fe6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75fe6-120">Header</span></span>|<span data-ttu-id="75fe6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75fe6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75fe6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75fe6-122">Authorization</span></span>|<span data-ttu-id="75fe6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75fe6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75fe6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75fe6-124">Accept</span></span>|<span data-ttu-id="75fe6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75fe6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75fe6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75fe6-126">Request body</span></span>
<span data-ttu-id="75fe6-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75fe6-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75fe6-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="75fe6-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75fe6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75fe6-129">Property</span></span>|<span data-ttu-id="75fe6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75fe6-130">Type</span></span>|<span data-ttu-id="75fe6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75fe6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75fe6-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="75fe6-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="75fe6-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="75fe6-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="75fe6-134">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="75fe6-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="75fe6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fe6-135">Response</span></span>
<span data-ttu-id="75fe6-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75fe6-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75fe6-137">Пример</span><span class="sxs-lookup"><span data-stu-id="75fe6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="75fe6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="75fe6-138">Request</span></span>
<span data-ttu-id="75fe6-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75fe6-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75fe6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fe6-140">Response</span></span>
<span data-ttu-id="75fe6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75fe6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




