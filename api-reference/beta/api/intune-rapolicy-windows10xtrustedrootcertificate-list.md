---
title: Список windows10XTrustedRootCertificates
description: Список свойств и связей объектов Windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75818cad36b196c8b3094bba2f558b3bd5b80454
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145077"
---
# <a name="list-windows10xtrustedrootcertificates"></a><span data-ttu-id="f1bfa-103">Список windows10XTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="f1bfa-103">List windows10XTrustedRootCertificates</span></span>

<span data-ttu-id="f1bfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1bfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1bfa-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1bfa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1bfa-107">Список свойств и связей [объектов Windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="f1bfa-107">List properties and relationships of the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1bfa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1bfa-108">Prerequisites</span></span>
<span data-ttu-id="f1bfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1bfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1bfa-111">Permission type</span></span>|<span data-ttu-id="f1bfa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1bfa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1bfa-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1bfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1bfa-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bfa-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1bfa-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1bfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1bfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-116">Not supported.</span></span>|
|<span data-ttu-id="f1bfa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1bfa-117">Application</span></span>|<span data-ttu-id="f1bfa-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bfa-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1bfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1bfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f1bfa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1bfa-120">Request headers</span></span>
|<span data-ttu-id="f1bfa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1bfa-121">Header</span></span>|<span data-ttu-id="f1bfa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1bfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1bfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1bfa-123">Authorization</span></span>|<span data-ttu-id="f1bfa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1bfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1bfa-125">Accept</span></span>|<span data-ttu-id="f1bfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1bfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1bfa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1bfa-127">Request body</span></span>
<span data-ttu-id="f1bfa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1bfa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1bfa-129">Response</span></span>
<span data-ttu-id="f1bfa-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1bfa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f1bfa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1bfa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1bfa-132">Request</span></span>
<span data-ttu-id="f1bfa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="f1bfa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1bfa-134">Response</span></span>
<span data-ttu-id="f1bfa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1bfa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 654

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
      "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value",
      "destinationStore": "computerCertStoreIntermediate"
    }
  ]
}
```




