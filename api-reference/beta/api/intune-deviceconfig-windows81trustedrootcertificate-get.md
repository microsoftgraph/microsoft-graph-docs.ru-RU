---
title: Получение windows81TrustedRootCertificate
description: Чтение свойств и связей объекта windows81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c61c108cb67f2a58535f0586b0dbe9de3eaae8f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163527"
---
# <a name="get-windows81trustedrootcertificate"></a><span data-ttu-id="98444-103">Получение windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="98444-103">Get windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="98444-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98444-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98444-106">Чтение свойств и связей объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="98444-106">Read properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98444-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98444-107">Prerequisites</span></span>
<span data-ttu-id="98444-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98444-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98444-110">Permission type</span></span>|<span data-ttu-id="98444-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98444-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98444-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98444-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98444-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98444-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="98444-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98444-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98444-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98444-115">Not supported.</span></span>|
|<span data-ttu-id="98444-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98444-116">Application</span></span>|<span data-ttu-id="98444-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98444-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98444-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98444-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98444-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98444-119">Optional query parameters</span></span>
<span data-ttu-id="98444-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98444-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98444-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98444-121">Request headers</span></span>
|<span data-ttu-id="98444-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98444-122">Header</span></span>|<span data-ttu-id="98444-123">Значение</span><span class="sxs-lookup"><span data-stu-id="98444-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98444-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98444-124">Authorization</span></span>|<span data-ttu-id="98444-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="98444-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98444-126">Accept</span><span class="sxs-lookup"><span data-stu-id="98444-126">Accept</span></span>|<span data-ttu-id="98444-127">application/json</span><span class="sxs-lookup"><span data-stu-id="98444-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98444-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98444-128">Request body</span></span>
<span data-ttu-id="98444-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98444-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98444-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="98444-130">Response</span></span>
<span data-ttu-id="98444-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98444-131">If successful, this method returns a `200 OK` response code and [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98444-132">Пример</span><span class="sxs-lookup"><span data-stu-id="98444-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="98444-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="98444-133">Request</span></span>
<span data-ttu-id="98444-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98444-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
```

### <a name="response"></a><span data-ttu-id="98444-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="98444-135">Response</span></span>
<span data-ttu-id="98444-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98444-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
    "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
    "certFileName": "Cert File Name value",
    "destinationStore": "computerCertStoreIntermediate"
  }
}
```




