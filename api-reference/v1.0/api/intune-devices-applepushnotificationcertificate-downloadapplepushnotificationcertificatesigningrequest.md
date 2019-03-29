---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09bbadd2e0874bdc461f965ff12544716e4de9d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970200"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="08fce-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="08fce-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="08fce-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08fce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08fce-105">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="08fce-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08fce-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08fce-106">Prerequisites</span></span>
<span data-ttu-id="08fce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08fce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08fce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08fce-109">Permission type</span></span>|<span data-ttu-id="08fce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08fce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08fce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08fce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08fce-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fce-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08fce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08fce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08fce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fce-114">Not supported.</span></span>|
|<span data-ttu-id="08fce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08fce-115">Application</span></span>|<span data-ttu-id="08fce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08fce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08fce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="08fce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08fce-118">Request headers</span></span>
|<span data-ttu-id="08fce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08fce-119">Header</span></span>|<span data-ttu-id="08fce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="08fce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08fce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08fce-121">Authorization</span></span>|<span data-ttu-id="08fce-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08fce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08fce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="08fce-123">Accept</span></span>|<span data-ttu-id="08fce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08fce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08fce-125">Request body</span></span>
<span data-ttu-id="08fce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08fce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08fce-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="08fce-127">Response</span></span>
<span data-ttu-id="08fce-128">В случае успеха эта функция возвращает код `200 OK` отклика и строку в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08fce-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fce-129">Пример</span><span class="sxs-lookup"><span data-stu-id="08fce-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="08fce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="08fce-130">Request</span></span>
<span data-ttu-id="08fce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08fce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="08fce-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fce-132">Response</span></span>
<span data-ttu-id="08fce-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08fce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



