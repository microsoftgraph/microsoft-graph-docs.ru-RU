---
title: 'Хранитель: Release'
description: Освобождение хранитель от случая.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 59e3ef5721c10419261443ca57d7584035dc1622
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597731"
---
# <a name="custodian-release"></a><span data-ttu-id="7b37d-103">Хранитель: Release</span><span class="sxs-lookup"><span data-stu-id="7b37d-103">custodian: release</span></span>

<span data-ttu-id="7b37d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b37d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b37d-105">Освобождение хранитель от случая.</span><span class="sxs-lookup"><span data-stu-id="7b37d-105">Release a custodian from a case.</span></span> <span data-ttu-id="7b37d-106">Дополнительную информацию можно узнать в статье [Release a хранитель из случая](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span><span class="sxs-lookup"><span data-stu-id="7b37d-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b37d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b37d-107">Permissions</span></span>

<span data-ttu-id="7b37d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b37d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b37d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b37d-110">Permission type</span></span>|<span data-ttu-id="7b37d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b37d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b37d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b37d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b37d-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="7b37d-113">User.Read</span></span>|
|<span data-ttu-id="7b37d-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b37d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b37d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b37d-115">Not supported.</span></span>|
|<span data-ttu-id="7b37d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b37d-116">Application</span></span>|<span data-ttu-id="7b37d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b37d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b37d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b37d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="7b37d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b37d-119">Request headers</span></span>

|<span data-ttu-id="7b37d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7b37d-120">Name</span></span>|<span data-ttu-id="7b37d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7b37d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b37d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b37d-122">Authorization</span></span>|<span data-ttu-id="7b37d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b37d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7b37d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b37d-125">Content-Type</span></span>|<span data-ttu-id="7b37d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b37d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b37d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b37d-128">Request body</span></span>

<span data-ttu-id="7b37d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b37d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b37d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b37d-130">Response</span></span>

<span data-ttu-id="7b37d-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b37d-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7b37d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b37d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b37d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b37d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```

### <a name="response"></a><span data-ttu-id="7b37d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b37d-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
