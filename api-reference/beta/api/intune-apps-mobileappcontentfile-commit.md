---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30ce7aee558c544aee29f1843d296e5e39ea8340
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149065"
---
# <a name="commit-action"></a><span data-ttu-id="6b7d2-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="6b7d2-103">commit action</span></span>

> <span data-ttu-id="6b7d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b7d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b7d2-106">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b7d2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6b7d2-107">Prerequisites</span></span>
<span data-ttu-id="6b7d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b7d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b7d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b7d2-110">Permission type</span></span>|<span data-ttu-id="6b7d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b7d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b7d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b7d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b7d2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7d2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b7d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b7d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b7d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-115">Not supported.</span></span>|
|<span data-ttu-id="6b7d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b7d2-116">Application</span></span>|<span data-ttu-id="6b7d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b7d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b7d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="6b7d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b7d2-119">Request headers</span></span>
|<span data-ttu-id="6b7d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b7d2-120">Header</span></span>|<span data-ttu-id="6b7d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b7d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b7d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b7d2-122">Authorization</span></span>|<span data-ttu-id="6b7d2-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6b7d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b7d2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b7d2-124">Accept</span></span>|<span data-ttu-id="6b7d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b7d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b7d2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b7d2-126">Request body</span></span>
<span data-ttu-id="6b7d2-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6b7d2-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6b7d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b7d2-129">Property</span></span>|<span data-ttu-id="6b7d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b7d2-130">Type</span></span>|<span data-ttu-id="6b7d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b7d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7d2-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="6b7d2-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="6b7d2-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="6b7d2-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="6b7d2-134">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="6b7d2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b7d2-135">Response</span></span>
<span data-ttu-id="6b7d2-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b7d2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6b7d2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b7d2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b7d2-138">Request</span></span>
<span data-ttu-id="6b7d2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b7d2-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b7d2-140">Response</span></span>
<span data-ttu-id="6b7d2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b7d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




