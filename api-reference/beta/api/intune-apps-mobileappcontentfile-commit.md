---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18242b7f4b3d874f85682d7a9eeb626455dea473
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797538"
---
# <a name="commit-action"></a><span data-ttu-id="aa7ac-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="aa7ac-103">commit action</span></span>

> <span data-ttu-id="aa7ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa7ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa7ac-106">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa7ac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa7ac-107">Prerequisites</span></span>
<span data-ttu-id="aa7ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa7ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa7ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa7ac-110">Permission type</span></span>|<span data-ttu-id="aa7ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa7ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa7ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa7ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa7ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa7ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aa7ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa7ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa7ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-115">Not supported.</span></span>|
|<span data-ttu-id="aa7ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa7ac-116">Application</span></span>|<span data-ttu-id="aa7ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa7ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa7ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="aa7ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa7ac-119">Request headers</span></span>
|<span data-ttu-id="aa7ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa7ac-120">Header</span></span>|<span data-ttu-id="aa7ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aa7ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa7ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa7ac-122">Authorization</span></span>|<span data-ttu-id="aa7ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa7ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aa7ac-124">Accept</span></span>|<span data-ttu-id="aa7ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa7ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa7ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa7ac-126">Request body</span></span>
<span data-ttu-id="aa7ac-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aa7ac-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa7ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa7ac-129">Property</span></span>|<span data-ttu-id="aa7ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aa7ac-130">Type</span></span>|<span data-ttu-id="aa7ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aa7ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa7ac-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="aa7ac-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="aa7ac-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="aa7ac-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="aa7ac-134">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="aa7ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa7ac-135">Response</span></span>
<span data-ttu-id="aa7ac-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa7ac-137">Пример</span><span class="sxs-lookup"><span data-stu-id="aa7ac-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa7ac-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa7ac-138">Request</span></span>
<span data-ttu-id="aa7ac-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa7ac-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa7ac-140">Response</span></span>
<span data-ttu-id="aa7ac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa7ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





