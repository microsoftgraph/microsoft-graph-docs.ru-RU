---
title: Получение Секуритибаселинетемплате
description: Чтение свойств и связей объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c484b78e17c92751c5ce8f0aa55006fe6e3145b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177172"
---
# <a name="get-securitybaselinetemplate"></a><span data-ttu-id="b9f6b-103">Получение Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="b9f6b-103">Get securityBaselineTemplate</span></span>

<span data-ttu-id="b9f6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f6b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f6b-107">Чтение свойств и связей объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f6b-107">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f6b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9f6b-108">Prerequisites</span></span>
<span data-ttu-id="b9f6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f6b-111">Permission type</span></span>|<span data-ttu-id="b9f6b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f6b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f6b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9f6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-116">Not supported.</span></span>|
|<span data-ttu-id="b9f6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f6b-117">Application</span></span>|<span data-ttu-id="b9f6b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f6b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f6b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9f6b-120">Optional query parameters</span></span>
<span data-ttu-id="b9f6b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f6b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f6b-122">Request headers</span></span>
|<span data-ttu-id="b9f6b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9f6b-123">Header</span></span>|<span data-ttu-id="b9f6b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b9f6b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f6b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9f6b-125">Authorization</span></span>|<span data-ttu-id="b9f6b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f6b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b9f6b-127">Accept</span></span>|<span data-ttu-id="b9f6b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f6b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f6b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9f6b-129">Request body</span></span>
<span data-ttu-id="b9f6b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f6b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9f6b-131">Response</span></span>
<span data-ttu-id="b9f6b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-132">If successful, this method returns a `200 OK` response code and [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f6b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f6b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f6b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f6b-134">Request</span></span>
<span data-ttu-id="b9f6b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="b9f6b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f6b-136">Response</span></span>
<span data-ttu-id="b9f6b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

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
    "templateSubtype": "firewall",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
  }
}
```



