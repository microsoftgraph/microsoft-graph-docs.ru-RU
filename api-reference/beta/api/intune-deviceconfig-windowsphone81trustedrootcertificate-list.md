---
title: Список windowsPhone81TrustedRootCertificates
description: Список свойств и связей объектов windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4347d38e8af1f63b734233c4e5cfd4b1c40b5836
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512651"
---
# <a name="list-windowsphone81trustedrootcertificates"></a><span data-ttu-id="113de-103">Список windowsPhone81TrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="113de-103">List windowsPhone81TrustedRootCertificates</span></span>

> <span data-ttu-id="113de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="113de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="113de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="113de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="113de-106">Список свойств и связей объектов [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="113de-106">List properties and relationships of the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="113de-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="113de-107">Prerequisites</span></span>
<span data-ttu-id="113de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="113de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="113de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="113de-110">Permission type</span></span>|<span data-ttu-id="113de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="113de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="113de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="113de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="113de-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="113de-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="113de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="113de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="113de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="113de-115">Not supported.</span></span>|
|<span data-ttu-id="113de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="113de-116">Application</span></span>|<span data-ttu-id="113de-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="113de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="113de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="113de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="113de-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="113de-119">Request headers</span></span>
|<span data-ttu-id="113de-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="113de-120">Header</span></span>|<span data-ttu-id="113de-121">Значение</span><span class="sxs-lookup"><span data-stu-id="113de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="113de-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="113de-122">Authorization</span></span>|<span data-ttu-id="113de-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="113de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="113de-124">Accept</span><span class="sxs-lookup"><span data-stu-id="113de-124">Accept</span></span>|<span data-ttu-id="113de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="113de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="113de-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="113de-126">Request body</span></span>
<span data-ttu-id="113de-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="113de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="113de-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="113de-128">Response</span></span>
<span data-ttu-id="113de-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="113de-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="113de-130">Пример</span><span class="sxs-lookup"><span data-stu-id="113de-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="113de-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="113de-131">Request</span></span>
<span data-ttu-id="113de-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="113de-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="113de-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="113de-133">Response</span></span>
<span data-ttu-id="113de-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="113de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 631

{
  "value": [
    {
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
  ]
}
```





