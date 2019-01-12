---
title: Список windows81TrustedRootCertificates
description: Свойства списка и связей объектов windows81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24d26f7808d6ff07a6897310d90d63e7b21be53b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948473"
---
# <a name="list-windows81trustedrootcertificates"></a><span data-ttu-id="de3b8-103">Список windows81TrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="de3b8-103">List windows81TrustedRootCertificates</span></span>

> <span data-ttu-id="de3b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de3b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de3b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de3b8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de3b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de3b8-107">Свойства списка и связей объектов [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="de3b8-107">List properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de3b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de3b8-108">Prerequisites</span></span>
<span data-ttu-id="de3b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de3b8-111">Permission type</span></span>|<span data-ttu-id="de3b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de3b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de3b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de3b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de3b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de3b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de3b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de3b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de3b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3b8-116">Not supported.</span></span>|
|<span data-ttu-id="de3b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de3b8-117">Application</span></span>|<span data-ttu-id="de3b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de3b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de3b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="de3b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de3b8-120">Request headers</span></span>
|<span data-ttu-id="de3b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de3b8-121">Header</span></span>|<span data-ttu-id="de3b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de3b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de3b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3b8-123">Authorization</span></span>|<span data-ttu-id="de3b8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="de3b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de3b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de3b8-125">Accept</span></span>|<span data-ttu-id="de3b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de3b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de3b8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de3b8-127">Request body</span></span>
<span data-ttu-id="de3b8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de3b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de3b8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="de3b8-129">Response</span></span>
<span data-ttu-id="de3b8-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="de3b8-130">If successful, this method returns a `200 OK` response code and a collection of [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de3b8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="de3b8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="de3b8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="de3b8-132">Request</span></span>
<span data-ttu-id="de3b8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de3b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

### <a name="response"></a><span data-ttu-id="de3b8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="de3b8-134">Response</span></span>
<span data-ttu-id="de3b8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="de3b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
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
  ]
}
```





