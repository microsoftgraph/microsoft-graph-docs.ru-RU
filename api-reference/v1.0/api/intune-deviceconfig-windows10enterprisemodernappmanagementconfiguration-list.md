---
title: Перечисление объектов windows10EnterpriseModernAppManagementConfiguration
description: Список свойств и связей объектов windows10EnterpriseModernAppManagementConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04e8c058646aec812889367fbaba76796a51e1b0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365427"
---
# <a name="list-windows10enterprisemodernappmanagementconfigurations"></a><span data-ttu-id="75b5b-103">Перечисление объектов windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="75b5b-103">List windows10EnterpriseModernAppManagementConfigurations</span></span>

> <span data-ttu-id="75b5b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75b5b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75b5b-105">Список свойств и связей объектов [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75b5b-105">List properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75b5b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75b5b-106">Prerequisites</span></span>
<span data-ttu-id="75b5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75b5b-109">Permission type</span></span>|<span data-ttu-id="75b5b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75b5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b5b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75b5b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75b5b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75b5b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75b5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75b5b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b5b-114">Not supported.</span></span>|
|<span data-ttu-id="75b5b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75b5b-115">Application</span></span>|<span data-ttu-id="75b5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75b5b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75b5b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75b5b-118">Request headers</span></span>
|<span data-ttu-id="75b5b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75b5b-119">Header</span></span>|<span data-ttu-id="75b5b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="75b5b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75b5b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75b5b-121">Authorization</span></span>|<span data-ttu-id="75b5b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75b5b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75b5b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="75b5b-123">Accept</span></span>|<span data-ttu-id="75b5b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="75b5b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b5b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75b5b-125">Request body</span></span>
<span data-ttu-id="75b5b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75b5b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75b5b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="75b5b-127">Response</span></span>
<span data-ttu-id="75b5b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75b5b-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b5b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="75b5b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="75b5b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="75b5b-130">Request</span></span>
<span data-ttu-id="75b5b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75b5b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="75b5b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="75b5b-132">Response</span></span>
<span data-ttu-id="75b5b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75b5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
      "id": "d6577687-7687-d657-8776-57d6877657d6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "uninstallBuiltInApps": true
    }
  ]
}
```




