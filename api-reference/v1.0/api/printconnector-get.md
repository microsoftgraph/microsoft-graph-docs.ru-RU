---
title: Get printConnector
description: Извлечение свойств и связей объекта соединители.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0d04dd07b5e3e6afa80f9104a223feb409b0e63b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517409"
---
# <a name="get-printconnector"></a><span data-ttu-id="f934c-103">Get printConnector</span><span class="sxs-lookup"><span data-stu-id="f934c-103">Get printConnector</span></span>
<span data-ttu-id="f934c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f934c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f934c-105">Извлечение свойств и связей объекта **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="f934c-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f934c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f934c-106">Permissions</span></span>
<span data-ttu-id="f934c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f934c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f934c-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f934c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f934c-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f934c-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f934c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f934c-111">Permission type</span></span> | <span data-ttu-id="f934c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f934c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f934c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f934c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f934c-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f934c-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="f934c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f934c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f934c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f934c-116">Not Supported.</span></span>|
|<span data-ttu-id="f934c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f934c-117">Application</span></span>|<span data-ttu-id="f934c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f934c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f934c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f934c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors/{printConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f934c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f934c-120">Optional query parameters</span></span>
<span data-ttu-id="f934c-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f934c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f934c-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f934c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f934c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f934c-123">Request headers</span></span>
|<span data-ttu-id="f934c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f934c-124">Name</span></span>|<span data-ttu-id="f934c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f934c-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f934c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f934c-126">Authorization</span></span>|<span data-ttu-id="f934c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f934c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f934c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f934c-129">Request body</span></span>
<span data-ttu-id="f934c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f934c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f934c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f934c-131">Response</span></span>

<span data-ttu-id="f934c-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printConnector](../resources/printconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f934c-132">If successful, this method returns a `200 OK` response code and a [printConnector](../resources/printconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f934c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f934c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f934c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f934c-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```


### <a name="response"></a><span data-ttu-id="f934c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f934c-135">Response</span></span>
<span data-ttu-id="f934c-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f934c-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

