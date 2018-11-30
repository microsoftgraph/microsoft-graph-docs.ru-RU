---
title: Действие renewUpload
description: Обновляет универсальный код ресурса SAS для отправки файла приложения.
ms.openlocfilehash: b2f94ddf98a41dd54348694fa65badd646e12d15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025531"
---
# <a name="renewupload-action"></a><span data-ttu-id="0fedb-103">Действие renewUpload</span><span class="sxs-lookup"><span data-stu-id="0fedb-103">renewUpload action</span></span>

> <span data-ttu-id="0fedb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0fedb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fedb-105">Обновляет универсальный код ресурса SAS для отправки файла приложения.</span><span class="sxs-lookup"><span data-stu-id="0fedb-105">Renews the SAS URI for an application file upload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fedb-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0fedb-106">Prerequisites</span></span>
<span data-ttu-id="0fedb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fedb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fedb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fedb-109">Permission type</span></span>|<span data-ttu-id="0fedb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fedb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fedb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fedb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0fedb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fedb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fedb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fedb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fedb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fedb-114">Not supported.</span></span>|
|<span data-ttu-id="0fedb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fedb-115">Application</span></span>|<span data-ttu-id="0fedb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fedb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fedb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fedb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

## <a name="request-headers"></a><span data-ttu-id="0fedb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fedb-118">Request headers</span></span>
|<span data-ttu-id="0fedb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fedb-119">Header</span></span>|<span data-ttu-id="0fedb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0fedb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fedb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fedb-121">Authorization</span></span>|<span data-ttu-id="0fedb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0fedb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fedb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0fedb-123">Accept</span></span>|<span data-ttu-id="0fedb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0fedb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fedb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fedb-125">Request body</span></span>
<span data-ttu-id="0fedb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fedb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fedb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fedb-127">Response</span></span>
<span data-ttu-id="0fedb-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0fedb-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0fedb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0fedb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fedb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fedb-130">Request</span></span>
<span data-ttu-id="0fedb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fedb-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

### <a name="response"></a><span data-ttu-id="0fedb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fedb-132">Response</span></span>
<span data-ttu-id="0fedb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0fedb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



