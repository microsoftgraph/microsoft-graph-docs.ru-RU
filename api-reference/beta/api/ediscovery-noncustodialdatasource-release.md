---
title: 'noncustodialDataSource: release'
description: Освобождает источник данных, не в отношении хранения, из дела.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9907ad3222af084cd349585f27df0a71221b22e6
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080830"
---
# <a name="noncustodialdatasource-release"></a><span data-ttu-id="7de2a-103">noncustodialDataSource: release</span><span class="sxs-lookup"><span data-stu-id="7de2a-103">noncustodialDataSource: release</span></span>

<span data-ttu-id="7de2a-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7de2a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de2a-105">Освобождает источник данных, не в отношении хранения, из дела.</span><span class="sxs-lookup"><span data-stu-id="7de2a-105">Releases the non-custodial data source from the case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7de2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7de2a-106">Permissions</span></span>

<span data-ttu-id="7de2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7de2a-109">Permission type</span></span>|<span data-ttu-id="7de2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7de2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7de2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7de2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7de2a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de2a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7de2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7de2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7de2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7de2a-114">Not supported.</span></span>|
|<span data-ttu-id="7de2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7de2a-115">Application</span></span>|<span data-ttu-id="7de2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7de2a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7de2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7de2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/Release
```

## <a name="request-headers"></a><span data-ttu-id="7de2a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7de2a-118">Request headers</span></span>

|<span data-ttu-id="7de2a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7de2a-119">Name</span></span>|<span data-ttu-id="7de2a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7de2a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7de2a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7de2a-121">Authorization</span></span>|<span data-ttu-id="7de2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7de2a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7de2a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7de2a-124">Request body</span></span>

<span data-ttu-id="7de2a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7de2a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7de2a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7de2a-126">Response</span></span>

<span data-ttu-id="7de2a-127">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7de2a-127">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7de2a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7de2a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7de2a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7de2a-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "noncustodialdatasource_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release
```

### <a name="response"></a><span data-ttu-id="7de2a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7de2a-130">Response</span></span>

<span data-ttu-id="7de2a-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7de2a-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
