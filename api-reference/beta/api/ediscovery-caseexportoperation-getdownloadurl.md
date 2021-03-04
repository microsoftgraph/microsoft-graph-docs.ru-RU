---
title: 'caseExportOperation: getDownloadUrl'
description: 'Возвращает URL-адрес загрузки '
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f05c7a63dce306ff07993e6111a9323c6a14d599
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447083"
---
# <a name="caseexportoperation-getdownloadurl"></a><span data-ttu-id="fac2b-103">caseExportOperation: getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="fac2b-103">caseExportOperation: getDownloadUrl</span></span>

<span data-ttu-id="fac2b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="fac2b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fac2b-105">Возвращает URL-адрес загрузки для экспорта, когда экспорт будет готов.</span><span class="sxs-lookup"><span data-stu-id="fac2b-105">Returns the download URL for an export when the export is ready.</span></span>

## <a name="permissions"></a><span data-ttu-id="fac2b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fac2b-106">Permissions</span></span>

<span data-ttu-id="fac2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fac2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fac2b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fac2b-109">Permission type</span></span>|<span data-ttu-id="fac2b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fac2b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fac2b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fac2b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fac2b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac2b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="fac2b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fac2b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fac2b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fac2b-114">Not supported.</span></span>|
|<span data-ttu-id="fac2b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fac2b-115">Application</span></span>|<span data-ttu-id="fac2b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fac2b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fac2b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fac2b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations/{operationId}/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="fac2b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fac2b-118">Request headers</span></span>
|<span data-ttu-id="fac2b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fac2b-119">Name</span></span>|<span data-ttu-id="fac2b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fac2b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fac2b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fac2b-121">Authorization</span></span>|<span data-ttu-id="fac2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fac2b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fac2b-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fac2b-124">Request body</span></span>
<span data-ttu-id="fac2b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fac2b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fac2b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fac2b-126">Response</span></span>

<span data-ttu-id="fac2b-127">В случае успешной работы эта функция возвращает код отклика и `200 OK` строку в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fac2b-127">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span> <span data-ttu-id="fac2b-128">Поле значения представляет URL-адрес загрузки, откуда можно извлечь экспорт.</span><span class="sxs-lookup"><span data-stu-id="fac2b-128">The value field represents the download URL from where the export can be retrieved.</span></span>

## <a name="examples"></a><span data-ttu-id="fac2b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="fac2b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fac2b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fac2b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "caseexportoperation_getdownloadurl"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

### <a name="response"></a><span data-ttu-id="fac2b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fac2b-131">Response</span></span>

<span data-ttu-id="fac2b-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fac2b-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://nam01pkgg0052.blob.edproxy.nam01.ediscovery.outlook.com/packaging0041e27c6c924a48befe348d34066c25/d0b6d2a7-5fc5-44f0-9bca-6b9d34a9410b.zip?sv=2018-03-28&sr=c&sig=TRFQNUGFtuVO7zd39oNJjzcQYJus2TXY%2B50aed4pJJM%3D&se=2020-12-28T23%3A06%3A26Z&sp=racwdl"
}
```
