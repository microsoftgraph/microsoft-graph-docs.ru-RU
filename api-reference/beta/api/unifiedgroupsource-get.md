---
title: Получение Унифиедграупсаурце
description: Чтение свойств и связей объекта Унифиедграупсаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f3867c3c649865d34f225dc2bd928aa1067b4f55
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597818"
---
# <a name="get-unifiedgroupsource"></a><span data-ttu-id="c80f8-103">Получение Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="c80f8-103">Get unifiedGroupSource</span></span>

<span data-ttu-id="c80f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c80f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c80f8-105">Чтение свойств и связей объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="c80f8-105">Read the properties and relationships of a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c80f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c80f8-106">Permissions</span></span>

<span data-ttu-id="c80f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c80f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c80f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c80f8-109">Permission type</span></span>|<span data-ttu-id="c80f8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c80f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c80f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c80f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c80f8-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c80f8-112">User.Read</span></span>|
|<span data-ttu-id="c80f8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c80f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c80f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c80f8-114">Not supported.</span></span>|
|<span data-ttu-id="c80f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c80f8-115">Application</span></span>|<span data-ttu-id="c80f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c80f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c80f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c80f8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c80f8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c80f8-118">Optional query parameters</span></span>

<span data-ttu-id="c80f8-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c80f8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c80f8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c80f8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c80f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c80f8-121">Request headers</span></span>

|<span data-ttu-id="c80f8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c80f8-122">Name</span></span>|<span data-ttu-id="c80f8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c80f8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c80f8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c80f8-124">Authorization</span></span>|<span data-ttu-id="c80f8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c80f8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c80f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c80f8-127">Request body</span></span>

<span data-ttu-id="c80f8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c80f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c80f8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80f8-129">Response</span></span>

<span data-ttu-id="c80f8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унифиедграупсаурце](../resources/unifiedgroupsource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c80f8-130">If successful, this method returns a `200 OK` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c80f8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c80f8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c80f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c80f8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

### <a name="response"></a><span data-ttu-id="c80f8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80f8-133">Response</span></span>

<span data-ttu-id="c80f8-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c80f8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "displayName": "Developers group",
    "createdDateTime": "2020-10-27T15:14:11.0048392Z",
    "id": "33434233-3030-3739-3043-393039324633",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "Megan Bowen"
        }
    }
}
```
