---
title: Получение Усерпфксцертификате
description: Чтение свойств и связей объекта Усерпфксцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 339f7662beae46c2c8513a59bd84c6b66d06a256
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527982"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="95803-103">Получение Усерпфксцертификате</span><span class="sxs-lookup"><span data-stu-id="95803-103">Get userPFXCertificate</span></span>

> <span data-ttu-id="95803-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95803-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95803-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95803-106">Чтение свойств и связей объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="95803-106">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95803-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95803-107">Prerequisites</span></span>
<span data-ttu-id="95803-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95803-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95803-110">Permission type</span></span>|<span data-ttu-id="95803-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95803-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95803-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95803-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95803-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95803-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95803-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95803-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95803-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95803-115">Not supported.</span></span>|
|<span data-ttu-id="95803-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95803-116">Application</span></span>|<span data-ttu-id="95803-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95803-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95803-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95803-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95803-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95803-119">Optional query parameters</span></span>
<span data-ttu-id="95803-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95803-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95803-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95803-121">Request headers</span></span>
|<span data-ttu-id="95803-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95803-122">Header</span></span>|<span data-ttu-id="95803-123">Значение</span><span class="sxs-lookup"><span data-stu-id="95803-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95803-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95803-124">Authorization</span></span>|<span data-ttu-id="95803-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95803-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95803-126">Accept</span><span class="sxs-lookup"><span data-stu-id="95803-126">Accept</span></span>|<span data-ttu-id="95803-127">application/json</span><span class="sxs-lookup"><span data-stu-id="95803-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95803-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95803-128">Request body</span></span>
<span data-ttu-id="95803-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95803-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95803-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="95803-130">Response</span></span>
<span data-ttu-id="95803-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95803-131">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95803-132">Пример</span><span class="sxs-lookup"><span data-stu-id="95803-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="95803-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="95803-133">Request</span></span>
<span data-ttu-id="95803-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95803-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="95803-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="95803-135">Response</span></span>
<span data-ttu-id="95803-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95803-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
    "@odata.type": "#microsoft.graph.userPFXCertificate",
    "id": "045c159b-159b-045c-9b15-5c049b155c04",
    "thumbprint": "Thumbprint value",
    "intendedPurpose": "smimeEncryption",
    "userPrincipalName": "User Principal Name value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "providerName": "Provider Name value",
    "keyName": "Key Name value",
    "paddingScheme": "pkcs1",
    "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



