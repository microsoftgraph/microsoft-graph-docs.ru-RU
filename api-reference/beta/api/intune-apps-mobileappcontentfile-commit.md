---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: tfitzmac
ms.openlocfilehash: c3993104334284c789db51c4306d562a4b89eacd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310705"
---
# <a name="commit-action"></a><span data-ttu-id="d7037-103">Действие commit</span><span class="sxs-lookup"><span data-stu-id="d7037-103">commit action</span></span>

> <span data-ttu-id="d7037-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7037-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7037-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7037-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7037-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7037-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7037-107">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="d7037-107">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7037-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7037-108">Prerequisites</span></span>
<span data-ttu-id="d7037-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7037-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7037-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7037-111">Permission type</span></span>|<span data-ttu-id="d7037-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7037-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7037-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7037-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7037-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7037-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7037-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7037-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7037-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7037-116">Not supported.</span></span>|
|<span data-ttu-id="d7037-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7037-117">Application</span></span>|<span data-ttu-id="d7037-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7037-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7037-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7037-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="d7037-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7037-120">Request headers</span></span>
|<span data-ttu-id="d7037-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7037-121">Header</span></span>|<span data-ttu-id="d7037-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7037-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7037-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7037-123">Authorization</span></span>|<span data-ttu-id="d7037-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7037-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7037-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7037-125">Accept</span></span>|<span data-ttu-id="d7037-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7037-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7037-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7037-127">Request body</span></span>
<span data-ttu-id="d7037-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7037-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d7037-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d7037-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d7037-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7037-130">Property</span></span>|<span data-ttu-id="d7037-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7037-131">Type</span></span>|<span data-ttu-id="d7037-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7037-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7037-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="d7037-133">fileEncryptionInfo</span></span>|[<span data-ttu-id="d7037-134">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="d7037-134">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="d7037-135">Ключ параметра сведений о шифровании файлов.</span><span class="sxs-lookup"><span data-stu-id="d7037-135">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="d7037-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7037-136">Response</span></span>
<span data-ttu-id="d7037-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d7037-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7037-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d7037-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7037-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7037-139">Request</span></span>
<span data-ttu-id="d7037-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7037-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7037-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7037-141">Response</span></span>
<span data-ttu-id="d7037-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7037-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





