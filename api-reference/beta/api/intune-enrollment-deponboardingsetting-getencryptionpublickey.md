---
title: функция getEncryptionPublicKey
description: Получение маркера открытого ключа, используемого для шифрования программы регистрации устройства Apple
ms.openlocfilehash: 3d15d1eb6655c97032100b131174b2ea356538e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075727"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="08467-103">функция getEncryptionPublicKey</span><span class="sxs-lookup"><span data-stu-id="08467-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="08467-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08467-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08467-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08467-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08467-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08467-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08467-107">Получение маркера открытого ключа, используемого для шифрования программы регистрации устройства Apple</span><span class="sxs-lookup"><span data-stu-id="08467-107">Get a public key to use to encrypt the Apple device enrollment program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08467-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08467-108">Prerequisites</span></span>
<span data-ttu-id="08467-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08467-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08467-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08467-111">Permission type</span></span>|<span data-ttu-id="08467-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08467-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08467-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08467-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08467-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="08467-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="08467-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08467-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08467-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08467-116">Not supported.</span></span>|
|<span data-ttu-id="08467-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08467-117">Application</span></span>|<span data-ttu-id="08467-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08467-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08467-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08467-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="08467-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08467-120">Request headers</span></span>
|<span data-ttu-id="08467-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08467-121">Header</span></span>|<span data-ttu-id="08467-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08467-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08467-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08467-123">Authorization</span></span>|<span data-ttu-id="08467-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08467-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08467-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08467-125">Accept</span></span>|<span data-ttu-id="08467-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08467-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08467-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08467-127">Request body</span></span>
<span data-ttu-id="08467-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08467-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08467-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="08467-129">Response</span></span>
<span data-ttu-id="08467-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08467-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08467-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08467-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="08467-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="08467-132">Request</span></span>
<span data-ttu-id="08467-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08467-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="08467-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="08467-134">Response</span></span>
<span data-ttu-id="08467-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="08467-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```





