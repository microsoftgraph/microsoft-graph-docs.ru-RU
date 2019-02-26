---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21cfc3872f25f808904ca3a96635bf715b0fc920
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252380"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="e26fb-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="e26fb-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="e26fb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e26fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e26fb-105">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="e26fb-105">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e26fb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e26fb-106">Prerequisites</span></span>
<span data-ttu-id="e26fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e26fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e26fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e26fb-109">Permission type</span></span>|<span data-ttu-id="e26fb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e26fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e26fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e26fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e26fb-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e26fb-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e26fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e26fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e26fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26fb-114">Not supported.</span></span>|
|<span data-ttu-id="e26fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e26fb-115">Application</span></span>|<span data-ttu-id="e26fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e26fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e26fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="e26fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e26fb-118">Request headers</span></span>
|<span data-ttu-id="e26fb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e26fb-119">Header</span></span>|<span data-ttu-id="e26fb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e26fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e26fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e26fb-121">Authorization</span></span>|<span data-ttu-id="e26fb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e26fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e26fb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e26fb-123">Accept</span></span>|<span data-ttu-id="e26fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e26fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e26fb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e26fb-125">Request body</span></span>
<span data-ttu-id="e26fb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e26fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e26fb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26fb-127">Response</span></span>
<span data-ttu-id="e26fb-128">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e26fb-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e26fb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e26fb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e26fb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e26fb-130">Request</span></span>
<span data-ttu-id="e26fb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e26fb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="e26fb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e26fb-132">Response</span></span>
<span data-ttu-id="e26fb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e26fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



