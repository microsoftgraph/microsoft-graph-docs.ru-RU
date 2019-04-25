---
title: Список Иострустедрутцертификатес
description: Список свойств и связей объектов Иострустедрутцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04450bb4f6445d30025aac0c6d74f84e29c38ac9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519411"
---
# <a name="list-iostrustedrootcertificates"></a><span data-ttu-id="13007-103">Список Иострустедрутцертификатес</span><span class="sxs-lookup"><span data-stu-id="13007-103">List iosTrustedRootCertificates</span></span>

> <span data-ttu-id="13007-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13007-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13007-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13007-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13007-106">Список свойств и связей объектов [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="13007-106">List properties and relationships of the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13007-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13007-107">Prerequisites</span></span>
<span data-ttu-id="13007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13007-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13007-110">Permission type</span></span>|<span data-ttu-id="13007-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13007-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13007-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13007-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13007-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13007-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13007-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13007-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13007-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13007-115">Not supported.</span></span>|
|<span data-ttu-id="13007-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13007-116">Application</span></span>|<span data-ttu-id="13007-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13007-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13007-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13007-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="13007-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13007-119">Request headers</span></span>
|<span data-ttu-id="13007-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13007-120">Header</span></span>|<span data-ttu-id="13007-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13007-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13007-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13007-122">Authorization</span></span>|<span data-ttu-id="13007-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13007-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13007-124">Accept</span><span class="sxs-lookup"><span data-stu-id="13007-124">Accept</span></span>|<span data-ttu-id="13007-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13007-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13007-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13007-126">Request body</span></span>
<span data-ttu-id="13007-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13007-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13007-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="13007-128">Response</span></span>
<span data-ttu-id="13007-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13007-129">If successful, this method returns a `200 OK` response code and a collection of [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13007-130">Пример</span><span class="sxs-lookup"><span data-stu-id="13007-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13007-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="13007-131">Request</span></span>
<span data-ttu-id="13007-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13007-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

### <a name="response"></a><span data-ttu-id="13007-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="13007-133">Response</span></span>
<span data-ttu-id="13007-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13007-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
      "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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
  ]
}
```





