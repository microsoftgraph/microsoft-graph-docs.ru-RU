---
title: Получение Ембеддедсимактиватионкодепул
description: Чтение свойств и связей объекта Ембеддедсимактиватионкодепул.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 989c8d1ae66fd1155a791b35dd4941ed4026ecfe
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184609"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="08257-103">Получение Ембеддедсимактиватионкодепул</span><span class="sxs-lookup"><span data-stu-id="08257-103">Get embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="08257-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08257-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08257-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08257-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08257-106">Чтение свойств и связей объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="08257-106">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08257-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08257-107">Prerequisites</span></span>
<span data-ttu-id="08257-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08257-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08257-110">Permission type</span></span>|<span data-ttu-id="08257-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08257-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08257-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08257-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08257-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08257-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="08257-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08257-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08257-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08257-115">Not supported.</span></span>|
|<span data-ttu-id="08257-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08257-116">Application</span></span>|<span data-ttu-id="08257-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08257-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08257-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08257-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08257-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08257-119">Optional query parameters</span></span>
<span data-ttu-id="08257-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08257-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08257-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08257-121">Request headers</span></span>
|<span data-ttu-id="08257-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08257-122">Header</span></span>|<span data-ttu-id="08257-123">Значение</span><span class="sxs-lookup"><span data-stu-id="08257-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08257-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08257-124">Authorization</span></span>|<span data-ttu-id="08257-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08257-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08257-126">Accept</span><span class="sxs-lookup"><span data-stu-id="08257-126">Accept</span></span>|<span data-ttu-id="08257-127">application/json</span><span class="sxs-lookup"><span data-stu-id="08257-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08257-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08257-128">Request body</span></span>
<span data-ttu-id="08257-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08257-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08257-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="08257-130">Response</span></span>
<span data-ttu-id="08257-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08257-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08257-132">Пример</span><span class="sxs-lookup"><span data-stu-id="08257-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="08257-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="08257-133">Request</span></span>
<span data-ttu-id="08257-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08257-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="08257-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="08257-135">Response</span></span>
<span data-ttu-id="08257-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08257-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
    "id": "ec308741-8741-ec30-4187-30ec418730ec",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "activationCodes": [
      {
        "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
        "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
        "matchingIdentifier": "Matching Identifier value",
        "smdpPlusServerAddress": "Smdp Plus Server Address value"
      }
    ],
    "activationCodeCount": 3
  }
}
```




