---
title: Получение Секуритибаселинетемплате
description: Чтение свойств и связей объекта Секуритибаселинетемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0c1528a3f3f209c048744a0ec9902b522461edd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945328"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="d38c4-103">Получение Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="d38c4-103">Get securityBaselineTemplate</span></span>

> <span data-ttu-id="d38c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d38c4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d38c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d38c4-106">Чтение свойств и связей объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="d38c4-106">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d38c4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d38c4-107">Prerequisites</span></span>
<span data-ttu-id="d38c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d38c4-110">Permission type</span></span>|<span data-ttu-id="d38c4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d38c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d38c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d38c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d38c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d38c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d38c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d38c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38c4-115">Not supported.</span></span>|
|<span data-ttu-id="d38c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d38c4-116">Application</span></span>|<span data-ttu-id="d38c4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38c4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d38c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d38c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d38c4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d38c4-119">Optional query parameters</span></span>
<span data-ttu-id="d38c4-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d38c4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d38c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d38c4-121">Request headers</span></span>
|<span data-ttu-id="d38c4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d38c4-122">Header</span></span>|<span data-ttu-id="d38c4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d38c4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d38c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d38c4-124">Authorization</span></span>|<span data-ttu-id="d38c4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d38c4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d38c4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d38c4-126">Accept</span></span>|<span data-ttu-id="d38c4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d38c4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d38c4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d38c4-128">Request body</span></span>
<span data-ttu-id="d38c4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d38c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d38c4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d38c4-130">Response</span></span>
<span data-ttu-id="d38c4-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d38c4-131">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38c4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d38c4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d38c4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d38c4-133">Request</span></span>
<span data-ttu-id="d38c4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d38c4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="d38c4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38c4-135">Response</span></span>
<span data-ttu-id="d38c4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d38c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineTemplate",
    "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
    "displayName": "Display Name value",
    "description": "Description value",
    "versionInfo": "Version Info value",
    "isDeprecated": true,
    "intentCount": 11,
    "templateType": "specializedDevices",
    "platformType": "androidForWork",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```





