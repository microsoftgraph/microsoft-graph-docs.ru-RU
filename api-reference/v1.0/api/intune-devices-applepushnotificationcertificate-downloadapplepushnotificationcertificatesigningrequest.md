---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c532c55386a25b23ca3cdc218a936b9f8e84adf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997010"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="08439-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="08439-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="08439-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08439-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08439-105">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="08439-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08439-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08439-106">Prerequisites</span></span>
<span data-ttu-id="08439-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08439-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08439-109">Permission type</span></span>|<span data-ttu-id="08439-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08439-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08439-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08439-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08439-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08439-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08439-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08439-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08439-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08439-114">Not supported.</span></span>|
|<span data-ttu-id="08439-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08439-115">Application</span></span>|<span data-ttu-id="08439-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08439-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08439-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08439-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="08439-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08439-118">Request headers</span></span>
|<span data-ttu-id="08439-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08439-119">Header</span></span>|<span data-ttu-id="08439-120">Значение</span><span class="sxs-lookup"><span data-stu-id="08439-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08439-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08439-121">Authorization</span></span>|<span data-ttu-id="08439-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08439-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08439-123">Accept</span><span class="sxs-lookup"><span data-stu-id="08439-123">Accept</span></span>|<span data-ttu-id="08439-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08439-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08439-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08439-125">Request body</span></span>
<span data-ttu-id="08439-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08439-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08439-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="08439-127">Response</span></span>
<span data-ttu-id="08439-128">В случае успеха эта функция возвращает код `200 OK` отклика и строку в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08439-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08439-129">Пример</span><span class="sxs-lookup"><span data-stu-id="08439-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="08439-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="08439-130">Request</span></span>
<span data-ttu-id="08439-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08439-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="08439-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="08439-132">Response</span></span>
<span data-ttu-id="08439-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08439-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



