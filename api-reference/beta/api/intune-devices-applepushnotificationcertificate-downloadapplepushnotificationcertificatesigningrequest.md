---
title: Функция downloadApplePushNotificationCertificateSigningRequest
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8fd7cbbbae02b56b13edcb05006ad2b5caf57d9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146748"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="f4cbb-103">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f4cbb-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="f4cbb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4cbb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4cbb-106">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="f4cbb-106">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4cbb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4cbb-107">Prerequisites</span></span>
<span data-ttu-id="f4cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4cbb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4cbb-110">Permission type</span></span>|<span data-ttu-id="f4cbb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4cbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4cbb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4cbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4cbb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cbb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4cbb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4cbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4cbb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-115">Not supported.</span></span>|
|<span data-ttu-id="f4cbb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4cbb-116">Application</span></span>|<span data-ttu-id="f4cbb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4cbb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4cbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="f4cbb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4cbb-119">Request headers</span></span>
|<span data-ttu-id="f4cbb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4cbb-120">Header</span></span>|<span data-ttu-id="f4cbb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4cbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4cbb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4cbb-122">Authorization</span></span>|<span data-ttu-id="f4cbb-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4cbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4cbb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4cbb-124">Accept</span></span>|<span data-ttu-id="f4cbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4cbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4cbb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4cbb-126">Request body</span></span>
<span data-ttu-id="f4cbb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4cbb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4cbb-128">Response</span></span>
<span data-ttu-id="f4cbb-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4cbb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f4cbb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4cbb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4cbb-131">Request</span></span>
<span data-ttu-id="f4cbb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="f4cbb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4cbb-133">Response</span></span>
<span data-ttu-id="f4cbb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4cbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```




