---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ffe34e641875a7c059f0c68f4471f17afa0f2cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978699"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="5c695-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="5c695-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="5c695-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c695-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c695-105">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="5c695-105">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c695-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c695-106">Prerequisites</span></span>
<span data-ttu-id="5c695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c695-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c695-109">Permission type</span></span>|<span data-ttu-id="5c695-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c695-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c695-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c695-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c695-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c695-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c695-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c695-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c695-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c695-114">Not supported.</span></span>|
|<span data-ttu-id="5c695-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c695-115">Application</span></span>|<span data-ttu-id="5c695-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c695-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c695-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c695-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="5c695-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c695-118">Request headers</span></span>
|<span data-ttu-id="5c695-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c695-119">Header</span></span>|<span data-ttu-id="5c695-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5c695-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c695-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c695-121">Authorization</span></span>|<span data-ttu-id="5c695-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c695-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c695-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5c695-123">Accept</span></span>|<span data-ttu-id="5c695-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c695-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c695-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c695-125">Request body</span></span>
<span data-ttu-id="5c695-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c695-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c695-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c695-127">Response</span></span>
<span data-ttu-id="5c695-128">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c695-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c695-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5c695-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c695-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c695-130">Request</span></span>
<span data-ttu-id="5c695-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c695-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="5c695-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c695-132">Response</span></span>
<span data-ttu-id="5c695-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c695-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



