---
title: Обновление printConnector
description: Обновление свойств объекта printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1fea6a1fe18012dcca1c266304e4430b1adcd660
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517404"
---
# <a name="update-printconnector"></a><span data-ttu-id="59656-103">Обновление printConnector</span><span class="sxs-lookup"><span data-stu-id="59656-103">Update printConnector</span></span>
<span data-ttu-id="59656-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="59656-105">Обновление свойств объекта **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="59656-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59656-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59656-106">Permissions</span></span>
<span data-ttu-id="59656-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="59656-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="59656-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="59656-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="59656-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="59656-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59656-111">Permission type</span></span> | <span data-ttu-id="59656-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59656-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="59656-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59656-113">Delegated (work or school account)</span></span>| <span data-ttu-id="59656-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59656-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="59656-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59656-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59656-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59656-116">Not Supported.</span></span>|
|<span data-ttu-id="59656-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="59656-117">Application</span></span>|<span data-ttu-id="59656-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59656-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59656-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59656-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="59656-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59656-120">Request headers</span></span>
|<span data-ttu-id="59656-121">Имя</span><span class="sxs-lookup"><span data-stu-id="59656-121">Name</span></span>|<span data-ttu-id="59656-122">Описание</span><span class="sxs-lookup"><span data-stu-id="59656-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59656-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59656-123">Authorization</span></span>|<span data-ttu-id="59656-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59656-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59656-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59656-126">Content-Type</span></span>|<span data-ttu-id="59656-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59656-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59656-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59656-129">Request body</span></span>
<span data-ttu-id="59656-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="59656-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="59656-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="59656-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59656-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="59656-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="59656-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59656-133">Response</span></span>
<span data-ttu-id="59656-134">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [printConnector](../resources/printConnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59656-134">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59656-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="59656-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59656-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="59656-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
Content-Type: application/json
Content-length: 308

{
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a><span data-ttu-id="59656-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="59656-137">Response</span></span>
<span data-ttu-id="59656-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59656-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

