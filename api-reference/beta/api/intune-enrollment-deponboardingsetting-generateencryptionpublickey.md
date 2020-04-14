---
title: действие Женератинкриптионпубликкэй
description: Создание открытого ключа, используемого для шифрования маркера программы регистрации устройств Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0bbabc3b3a6e0d8f150e7978c441a05381c9b41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444783"
---
# <a name="generateencryptionpublickey-action"></a><span data-ttu-id="0aac7-103">действие Женератинкриптионпубликкэй</span><span class="sxs-lookup"><span data-stu-id="0aac7-103">generateEncryptionPublicKey action</span></span>

<span data-ttu-id="0aac7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aac7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aac7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aac7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aac7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0aac7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aac7-107">Создание открытого ключа, используемого для шифрования маркера программы регистрации устройств Apple</span><span class="sxs-lookup"><span data-stu-id="0aac7-107">Generate a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aac7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0aac7-108">Prerequisites</span></span>
<span data-ttu-id="0aac7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aac7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0aac7-111">Permission type</span></span>|<span data-ttu-id="0aac7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0aac7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aac7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0aac7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0aac7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aac7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0aac7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0aac7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aac7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aac7-116">Not supported.</span></span>|
|<span data-ttu-id="0aac7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0aac7-117">Application</span></span>|<span data-ttu-id="0aac7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aac7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aac7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0aac7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/generateEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="0aac7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0aac7-120">Request headers</span></span>
|<span data-ttu-id="0aac7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0aac7-121">Header</span></span>|<span data-ttu-id="0aac7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0aac7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aac7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aac7-123">Authorization</span></span>|<span data-ttu-id="0aac7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0aac7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aac7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0aac7-125">Accept</span></span>|<span data-ttu-id="0aac7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0aac7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aac7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0aac7-127">Request body</span></span>
<span data-ttu-id="0aac7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0aac7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aac7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0aac7-129">Response</span></span>
<span data-ttu-id="0aac7-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0aac7-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aac7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0aac7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aac7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0aac7-132">Request</span></span>
<span data-ttu-id="0aac7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0aac7-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/generateEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="0aac7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aac7-134">Response</span></span>
<span data-ttu-id="0aac7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0aac7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 55

{
  "value": "Generate Encryption Public Key value"
}
```



