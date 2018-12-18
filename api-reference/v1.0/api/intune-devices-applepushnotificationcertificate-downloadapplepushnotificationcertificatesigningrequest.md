---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
ms.openlocfilehash: 99a62c456dd8d4f0e0779c44b800169e5de57164
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315521"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="fe08c-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="fe08c-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="fe08c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe08c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe08c-105">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="fe08c-105">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe08c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe08c-106">Prerequisites</span></span>
<span data-ttu-id="fe08c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe08c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe08c-109">Permission type</span></span>|<span data-ttu-id="fe08c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe08c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe08c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe08c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe08c-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe08c-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe08c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe08c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe08c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe08c-114">Not supported.</span></span>|
|<span data-ttu-id="fe08c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe08c-115">Application</span></span>|<span data-ttu-id="fe08c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe08c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe08c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe08c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="fe08c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe08c-118">Request headers</span></span>
|<span data-ttu-id="fe08c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe08c-119">Header</span></span>|<span data-ttu-id="fe08c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fe08c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe08c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe08c-121">Authorization</span></span>|<span data-ttu-id="fe08c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe08c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe08c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fe08c-123">Accept</span></span>|<span data-ttu-id="fe08c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe08c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe08c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe08c-125">Request body</span></span>
<span data-ttu-id="fe08c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe08c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe08c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe08c-127">Response</span></span>
<span data-ttu-id="fe08c-128">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe08c-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe08c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fe08c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe08c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe08c-130">Request</span></span>
<span data-ttu-id="fe08c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe08c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="fe08c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe08c-132">Response</span></span>
<span data-ttu-id="fe08c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe08c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



