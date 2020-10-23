---
title: действие Женератеапплепушнотификатионцертификатесигнингрекуест
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 037f0e109239ae98daa16552ecef176169ebd30b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723261"
---
# <a name="generateapplepushnotificationcertificatesigningrequest-action"></a><span data-ttu-id="33038-103">действие Женератеапплепушнотификатионцертификатесигнингрекуест</span><span class="sxs-lookup"><span data-stu-id="33038-103">generateApplePushNotificationCertificateSigningRequest action</span></span>

<span data-ttu-id="33038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33038-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33038-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33038-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33038-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33038-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33038-107">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="33038-107">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33038-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33038-108">Prerequisites</span></span>
<span data-ttu-id="33038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33038-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33038-111">Permission type</span></span>|<span data-ttu-id="33038-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33038-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33038-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33038-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33038-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33038-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="33038-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33038-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33038-116">Not supported.</span></span>|
|<span data-ttu-id="33038-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33038-117">Application</span></span>|<span data-ttu-id="33038-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33038-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33038-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33038-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="33038-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33038-120">Request headers</span></span>
|<span data-ttu-id="33038-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33038-121">Header</span></span>|<span data-ttu-id="33038-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33038-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33038-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33038-123">Authorization</span></span>|<span data-ttu-id="33038-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33038-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33038-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33038-125">Accept</span></span>|<span data-ttu-id="33038-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33038-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33038-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33038-127">Request body</span></span>
<span data-ttu-id="33038-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33038-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33038-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="33038-129">Response</span></span>
<span data-ttu-id="33038-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33038-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33038-131">Пример</span><span class="sxs-lookup"><span data-stu-id="33038-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33038-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33038-132">Request</span></span>
<span data-ttu-id="33038-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33038-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="33038-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33038-134">Response</span></span>
<span data-ttu-id="33038-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33038-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Generate Apple Push Notification Certificate Signing Request value"
}
```





