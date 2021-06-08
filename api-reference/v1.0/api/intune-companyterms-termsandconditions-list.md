---
title: Перечисление объектов termsAndConditions
description: Список свойств и связей объектов termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78d00f608e6ca4274e7f5753b4c7ba8e42e914bf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758416"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="3e00e-103">Перечисление объектов termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3e00e-103">List termsAndConditionses</span></span>

<span data-ttu-id="3e00e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e00e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e00e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e00e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e00e-106">Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3e00e-106">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e00e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e00e-107">Prerequisites</span></span>
<span data-ttu-id="3e00e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e00e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e00e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e00e-110">Permission type</span></span>|<span data-ttu-id="3e00e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e00e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e00e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e00e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e00e-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e00e-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e00e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e00e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e00e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e00e-115">Not supported.</span></span>|
|<span data-ttu-id="3e00e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e00e-116">Application</span></span>|<span data-ttu-id="3e00e-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e00e-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e00e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e00e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="3e00e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e00e-119">Request headers</span></span>
|<span data-ttu-id="3e00e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e00e-120">Header</span></span>|<span data-ttu-id="3e00e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e00e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e00e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e00e-122">Authorization</span></span>|<span data-ttu-id="3e00e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e00e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e00e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e00e-124">Accept</span></span>|<span data-ttu-id="3e00e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e00e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e00e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e00e-126">Request body</span></span>
<span data-ttu-id="3e00e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e00e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e00e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e00e-128">Response</span></span>
<span data-ttu-id="3e00e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e00e-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e00e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3e00e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e00e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e00e-131">Request</span></span>
<span data-ttu-id="3e00e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e00e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="3e00e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e00e-133">Response</span></span>
<span data-ttu-id="3e00e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e00e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```




