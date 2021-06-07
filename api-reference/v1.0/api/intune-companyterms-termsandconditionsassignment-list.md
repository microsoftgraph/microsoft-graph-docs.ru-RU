---
title: Перечисление объектов termsAndConditionsAssignment
description: Список свойств и связей объектов termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 025dd248aaaf91703a356f1a36b2796dd6972e19
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756708"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="ed922-103">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="ed922-103">List termsAndConditionsAssignments</span></span>

<span data-ttu-id="ed922-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed922-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed922-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed922-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed922-106">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ed922-106">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed922-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ed922-107">Prerequisites</span></span>
<span data-ttu-id="ed922-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed922-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed922-110">Permission type</span></span>|<span data-ttu-id="ed922-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed922-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed922-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed922-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed922-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed922-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed922-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed922-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed922-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed922-115">Not supported.</span></span>|
|<span data-ttu-id="ed922-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ed922-116">Application</span></span>|<span data-ttu-id="ed922-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed922-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed922-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed922-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ed922-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ed922-119">Request headers</span></span>
|<span data-ttu-id="ed922-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed922-120">Header</span></span>|<span data-ttu-id="ed922-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ed922-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed922-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed922-122">Authorization</span></span>|<span data-ttu-id="ed922-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed922-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed922-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ed922-124">Accept</span></span>|<span data-ttu-id="ed922-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed922-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed922-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed922-126">Request body</span></span>
<span data-ttu-id="ed922-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed922-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed922-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed922-128">Response</span></span>
<span data-ttu-id="ed922-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed922-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed922-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ed922-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed922-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed922-131">Request</span></span>
<span data-ttu-id="ed922-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed922-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="ed922-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed922-133">Response</span></span>
<span data-ttu-id="ed922-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed922-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




