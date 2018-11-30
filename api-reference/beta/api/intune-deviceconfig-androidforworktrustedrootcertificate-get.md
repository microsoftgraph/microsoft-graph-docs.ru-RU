---
title: Получение androidForWorkTrustedRootCertificate
description: Чтение свойства и связи объекта androidForWorkTrustedRootCertificate.
ms.openlocfilehash: ae3db38cea96c2e895b32d03df7f4f2e5cbde6c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078572"
---
# <a name="get-androidforworktrustedrootcertificate"></a><span data-ttu-id="53d98-103">Получение androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="53d98-103">Get androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="53d98-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53d98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53d98-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53d98-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53d98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53d98-107">Чтение свойства и связи объекта [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="53d98-107">Read properties and relationships of the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53d98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53d98-108">Prerequisites</span></span>
<span data-ttu-id="53d98-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53d98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53d98-111">Permission type</span></span>|<span data-ttu-id="53d98-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53d98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53d98-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53d98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53d98-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="53d98-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="53d98-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53d98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53d98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d98-116">Not supported.</span></span>|
|<span data-ttu-id="53d98-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53d98-117">Application</span></span>|<span data-ttu-id="53d98-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d98-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53d98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53d98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53d98-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53d98-120">Optional query parameters</span></span>
<span data-ttu-id="53d98-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53d98-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53d98-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53d98-122">Request headers</span></span>
|<span data-ttu-id="53d98-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53d98-123">Header</span></span>|<span data-ttu-id="53d98-124">Значение</span><span class="sxs-lookup"><span data-stu-id="53d98-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53d98-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d98-125">Authorization</span></span>|<span data-ttu-id="53d98-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53d98-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53d98-127">Accept</span><span class="sxs-lookup"><span data-stu-id="53d98-127">Accept</span></span>|<span data-ttu-id="53d98-128">application/json</span><span class="sxs-lookup"><span data-stu-id="53d98-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53d98-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53d98-129">Request body</span></span>
<span data-ttu-id="53d98-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53d98-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d98-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="53d98-131">Response</span></span>
<span data-ttu-id="53d98-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53d98-132">If successful, this method returns a `200 OK` response code and [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53d98-133">Пример</span><span class="sxs-lookup"><span data-stu-id="53d98-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="53d98-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53d98-134">Request</span></span>
<span data-ttu-id="53d98-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53d98-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
```

### <a name="response"></a><span data-ttu-id="53d98-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="53d98-136">Response</span></span>
<span data-ttu-id="53d98-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="53d98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 591

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
    "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value"
  }
}
```





