---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
ms.openlocfilehash: 12ceee63ab753c0540e0a8df7dfeff0e62de5748
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078406"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="01e56-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="01e56-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="01e56-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01e56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01e56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01e56-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01e56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01e56-107">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="01e56-107">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01e56-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01e56-108">Prerequisites</span></span>
<span data-ttu-id="01e56-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01e56-111">Permission type</span></span>|<span data-ttu-id="01e56-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01e56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01e56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01e56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01e56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="01e56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01e56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01e56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e56-116">Not supported.</span></span>|
|<span data-ttu-id="01e56-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01e56-117">Application</span></span>|<span data-ttu-id="01e56-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01e56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01e56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="01e56-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01e56-120">Request headers</span></span>
|<span data-ttu-id="01e56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01e56-121">Header</span></span>|<span data-ttu-id="01e56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01e56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01e56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01e56-123">Authorization</span></span>|<span data-ttu-id="01e56-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01e56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01e56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01e56-125">Accept</span></span>|<span data-ttu-id="01e56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01e56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01e56-127">Request body</span></span>
<span data-ttu-id="01e56-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01e56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01e56-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e56-129">Response</span></span>
<span data-ttu-id="01e56-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01e56-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="01e56-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="01e56-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="01e56-132">Request</span></span>
<span data-ttu-id="01e56-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01e56-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="01e56-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="01e56-134">Response</span></span>
<span data-ttu-id="01e56-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="01e56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```





