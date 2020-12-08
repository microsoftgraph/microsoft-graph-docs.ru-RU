---
title: Удаление Ситесаурце
description: Удаление объекта Ситесаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 26e8795582777e6a1e01d60ea25b902330af30aa
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597735"
---
# <a name="delete-sitesource"></a><span data-ttu-id="e8dd4-103">Удаление Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="e8dd4-103">Delete siteSource</span></span>

<span data-ttu-id="e8dd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8dd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8dd4-105">Удаление объекта [ситесаурце](../resources/sitesource.md) .</span><span class="sxs-lookup"><span data-stu-id="e8dd4-105">Delete a [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8dd4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8dd4-106">Permissions</span></span>

<span data-ttu-id="e8dd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8dd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8dd4-109">Permission type</span></span>|<span data-ttu-id="e8dd4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8dd4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8dd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8dd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8dd4-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="e8dd4-112">User.Read</span></span>|
|<span data-ttu-id="e8dd4-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8dd4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8dd4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8dd4-114">Not supported.</span></span>|
|<span data-ttu-id="e8dd4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8dd4-115">Application</span></span>|<span data-ttu-id="e8dd4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8dd4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8dd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8dd4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="e8dd4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8dd4-118">Request headers</span></span>

|<span data-ttu-id="e8dd4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8dd4-119">Name</span></span>|<span data-ttu-id="e8dd4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8dd4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8dd4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8dd4-121">Authorization</span></span>|<span data-ttu-id="e8dd4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8dd4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dd4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8dd4-124">Request body</span></span>

<span data-ttu-id="e8dd4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8dd4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8dd4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8dd4-126">Response</span></span>

<span data-ttu-id="e8dd4-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8dd4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8dd4-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8dd4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8dd4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8dd4-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```

### <a name="response"></a><span data-ttu-id="e8dd4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8dd4-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
