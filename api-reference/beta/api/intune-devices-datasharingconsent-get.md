---
title: Получение Даташарингконсент
description: Чтение свойств и связей объекта Даташарингконсент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7bbfd26af56734b62385a37157832f94994c6949
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981747"
---
# <a name="get-datasharingconsent"></a><span data-ttu-id="d192d-103">Получение Даташарингконсент</span><span class="sxs-lookup"><span data-stu-id="d192d-103">Get dataSharingConsent</span></span>

> <span data-ttu-id="d192d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d192d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d192d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d192d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d192d-106">Чтение свойств и связей объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="d192d-106">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d192d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d192d-107">Prerequisites</span></span>
<span data-ttu-id="d192d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d192d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d192d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d192d-110">Permission type</span></span>|<span data-ttu-id="d192d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d192d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d192d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d192d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d192d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d192d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d192d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d192d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d192d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d192d-115">Not supported.</span></span>|
|<span data-ttu-id="d192d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d192d-116">Application</span></span>|<span data-ttu-id="d192d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d192d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d192d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d192d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d192d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d192d-119">Optional query parameters</span></span>
<span data-ttu-id="d192d-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d192d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d192d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d192d-121">Request headers</span></span>
|<span data-ttu-id="d192d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d192d-122">Header</span></span>|<span data-ttu-id="d192d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d192d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d192d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d192d-124">Authorization</span></span>|<span data-ttu-id="d192d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d192d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d192d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d192d-126">Accept</span></span>|<span data-ttu-id="d192d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d192d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d192d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d192d-128">Request body</span></span>
<span data-ttu-id="d192d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d192d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d192d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d192d-130">Response</span></span>
<span data-ttu-id="d192d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [даташарингконсент](../resources/intune-devices-datasharingconsent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d192d-131">If successful, this method returns a `200 OK` response code and [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d192d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d192d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d192d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d192d-133">Request</span></span>
<span data-ttu-id="d192d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d192d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="d192d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d192d-135">Response</span></span>
<span data-ttu-id="d192d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d192d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```





