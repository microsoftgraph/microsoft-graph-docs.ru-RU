---
title: Получение windowsPhone81TrustedRootCertificate
description: Чтение свойства и связи объекта windowsPhone81TrustedRootCertificate.
author: tfitzmac
ms.openlocfilehash: 1bfb8c7e92c40cb6194dbcae1d56add7bbf0fc84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355083"
---
# <a name="get-windowsphone81trustedrootcertificate"></a><span data-ttu-id="87557-103">Получение windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="87557-103">Get windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="87557-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87557-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87557-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87557-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87557-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87557-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87557-107">Чтение свойства и связи объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="87557-107">Read properties and relationships of the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87557-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87557-108">Prerequisites</span></span>
<span data-ttu-id="87557-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87557-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87557-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87557-111">Permission type</span></span>|<span data-ttu-id="87557-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87557-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87557-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87557-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87557-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87557-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87557-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87557-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87557-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87557-116">Not supported.</span></span>|
|<span data-ttu-id="87557-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87557-117">Application</span></span>|<span data-ttu-id="87557-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87557-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87557-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87557-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87557-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87557-120">Optional query parameters</span></span>
<span data-ttu-id="87557-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87557-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87557-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87557-122">Request headers</span></span>
|<span data-ttu-id="87557-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87557-123">Header</span></span>|<span data-ttu-id="87557-124">Значение</span><span class="sxs-lookup"><span data-stu-id="87557-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87557-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87557-125">Authorization</span></span>|<span data-ttu-id="87557-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87557-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87557-127">Accept</span><span class="sxs-lookup"><span data-stu-id="87557-127">Accept</span></span>|<span data-ttu-id="87557-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87557-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87557-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87557-129">Request body</span></span>
<span data-ttu-id="87557-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87557-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87557-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="87557-131">Response</span></span>
<span data-ttu-id="87557-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87557-132">If successful, this method returns a `200 OK` response code and [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87557-133">Пример</span><span class="sxs-lookup"><span data-stu-id="87557-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="87557-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="87557-134">Request</span></span>
<span data-ttu-id="87557-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87557-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="87557-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="87557-136">Response</span></span>
<span data-ttu-id="87557-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87557-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 591

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
    "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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





