---
title: Действие renewUpload
description: Обновляет универсальный код ресурса SAS для отправки файла приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e68ae93113db49fe7bd8c12d335406db2f4a18b1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975058"
---
# <a name="renewupload-action"></a><span data-ttu-id="7a7ab-103">Действие renewUpload</span><span class="sxs-lookup"><span data-stu-id="7a7ab-103">renewUpload action</span></span>

> <span data-ttu-id="7a7ab-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a7ab-105">Обновляет универсальный код ресурса SAS для отправки файла приложения.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-105">Renews the SAS URI for an application file upload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a7ab-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7a7ab-106">Prerequisites</span></span>
<span data-ttu-id="7a7ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a7ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a7ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a7ab-109">Permission type</span></span>|<span data-ttu-id="7a7ab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a7ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a7ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a7ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a7ab-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a7ab-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a7ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a7ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a7ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-114">Not supported.</span></span>|
|<span data-ttu-id="7a7ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a7ab-115">Application</span></span>|<span data-ttu-id="7a7ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a7ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a7ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

## <a name="request-headers"></a><span data-ttu-id="7a7ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a7ab-118">Request headers</span></span>
|<span data-ttu-id="7a7ab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a7ab-119">Header</span></span>|<span data-ttu-id="7a7ab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7a7ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a7ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a7ab-121">Authorization</span></span>|<span data-ttu-id="7a7ab-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a7ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7a7ab-123">Accept</span></span>|<span data-ttu-id="7a7ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a7ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a7ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a7ab-125">Request body</span></span>
<span data-ttu-id="7a7ab-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a7ab-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a7ab-127">Response</span></span>
<span data-ttu-id="7a7ab-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a7ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7a7ab-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a7ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a7ab-130">Request</span></span>
<span data-ttu-id="7a7ab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

### <a name="response"></a><span data-ttu-id="7a7ab-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a7ab-132">Response</span></span>
<span data-ttu-id="7a7ab-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a7ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



