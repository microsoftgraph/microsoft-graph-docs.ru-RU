---
title: действие Женератеапплепушнотификатионцертификатесигнингрекуест
description: Скачивание запроса на подпись сертификата для push-уведомлений Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4b602e3819f799493a69619309580acb7cc6e77
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427057"
---
# <a name="generateapplepushnotificationcertificatesigningrequest-action"></a><span data-ttu-id="ebacc-103">действие Женератеапплепушнотификатионцертификатесигнингрекуест</span><span class="sxs-lookup"><span data-stu-id="ebacc-103">generateApplePushNotificationCertificateSigningRequest action</span></span>

<span data-ttu-id="ebacc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebacc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebacc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebacc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebacc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebacc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebacc-107">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="ebacc-107">Download Apple push notification certificate signing request</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebacc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ebacc-108">Prerequisites</span></span>
<span data-ttu-id="ebacc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebacc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebacc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebacc-111">Permission type</span></span>|<span data-ttu-id="ebacc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebacc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebacc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebacc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebacc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebacc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebacc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebacc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebacc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebacc-116">Not supported.</span></span>|
|<span data-ttu-id="ebacc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebacc-117">Application</span></span>|<span data-ttu-id="ebacc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebacc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebacc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebacc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="ebacc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ebacc-120">Request headers</span></span>
|<span data-ttu-id="ebacc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebacc-121">Header</span></span>|<span data-ttu-id="ebacc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ebacc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebacc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebacc-123">Authorization</span></span>|<span data-ttu-id="ebacc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebacc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebacc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ebacc-125">Accept</span></span>|<span data-ttu-id="ebacc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebacc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebacc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebacc-127">Request body</span></span>
<span data-ttu-id="ebacc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebacc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebacc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebacc-129">Response</span></span>
<span data-ttu-id="ebacc-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebacc-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebacc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ebacc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebacc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebacc-132">Request</span></span>
<span data-ttu-id="ebacc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebacc-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="ebacc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebacc-134">Response</span></span>
<span data-ttu-id="ebacc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebacc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Generate Apple Push Notification Certificate Signing Request value"
}
```



