---
title: Действие createDownloadUrl
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed7e111dc99e3db3f44accdbaaee9b205e8c5ae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164122"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="36d50-103">Действие createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="36d50-103">createDownloadUrl action</span></span>

> <span data-ttu-id="36d50-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36d50-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36d50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d50-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36d50-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36d50-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36d50-107">Prerequisites</span></span>
<span data-ttu-id="36d50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="36d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36d50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36d50-110">Permission type</span></span>|<span data-ttu-id="36d50-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36d50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36d50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36d50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36d50-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="36d50-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="36d50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36d50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36d50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d50-115">Not supported.</span></span>|
|<span data-ttu-id="36d50-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36d50-116">Application</span></span>|<span data-ttu-id="36d50-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36d50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36d50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="36d50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36d50-119">Request headers</span></span>
|<span data-ttu-id="36d50-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36d50-120">Header</span></span>|<span data-ttu-id="36d50-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36d50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36d50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36d50-122">Authorization</span></span>|<span data-ttu-id="36d50-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36d50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36d50-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36d50-124">Accept</span></span>|<span data-ttu-id="36d50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36d50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d50-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36d50-126">Request body</span></span>
<span data-ttu-id="36d50-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36d50-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36d50-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="36d50-128">Response</span></span>
<span data-ttu-id="36d50-129">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [апплогколлектиондовнлоаддетаилс](../resources/intune-devices-applogcollectiondownloaddetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36d50-129">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d50-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36d50-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="36d50-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36d50-131">Request</span></span>
<span data-ttu-id="36d50-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36d50-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="36d50-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="36d50-133">Response</span></span>
<span data-ttu-id="36d50-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36d50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
    "downloadUrl": "https://example.com/downloadUrl/",
    "decryptionKey": "Decryption Key value",
    "appLogDecryptionAlgorithm": "aes256"
  }
}
```




