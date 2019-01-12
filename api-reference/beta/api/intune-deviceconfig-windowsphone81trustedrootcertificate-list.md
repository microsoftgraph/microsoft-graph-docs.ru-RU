---
title: Список windowsPhone81TrustedRootCertificates
description: Свойства списка и связей объектов windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d3f9ee4bcfff4e38bf8dac2193b738c3d6ba1787
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964902"
---
# <a name="list-windowsphone81trustedrootcertificates"></a><span data-ttu-id="c87b3-103">Список windowsPhone81TrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="c87b3-103">List windowsPhone81TrustedRootCertificates</span></span>

> <span data-ttu-id="c87b3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c87b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c87b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c87b3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c87b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c87b3-107">Свойства списка и связей объектов [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c87b3-107">List properties and relationships of the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c87b3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c87b3-108">Prerequisites</span></span>
<span data-ttu-id="c87b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c87b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c87b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c87b3-111">Permission type</span></span>|<span data-ttu-id="c87b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c87b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c87b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c87b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c87b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c87b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c87b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c87b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87b3-116">Not supported.</span></span>|
|<span data-ttu-id="c87b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c87b3-117">Application</span></span>|<span data-ttu-id="c87b3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c87b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c87b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c87b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c87b3-120">Request headers</span></span>
|<span data-ttu-id="c87b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c87b3-121">Header</span></span>|<span data-ttu-id="c87b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c87b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c87b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c87b3-123">Authorization</span></span>|<span data-ttu-id="c87b3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c87b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c87b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c87b3-125">Accept</span></span>|<span data-ttu-id="c87b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c87b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c87b3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c87b3-127">Request body</span></span>
<span data-ttu-id="c87b3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c87b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c87b3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c87b3-129">Response</span></span>
<span data-ttu-id="c87b3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c87b3-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c87b3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c87b3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c87b3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87b3-132">Request</span></span>
<span data-ttu-id="c87b3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c87b3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c87b3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c87b3-134">Response</span></span>
<span data-ttu-id="c87b3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c87b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





