---
title: Удаление Унифиедграупсаурце
description: Удаление объекта Унифиедграупсаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e2eb86c566703e6c23262a0ddb572e438d33ce
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597824"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="e6a6f-103">Удаление Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e6a6f-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="e6a6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6a6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6a6f-105">Удаление объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="e6a6f-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6a6f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a6f-106">Permissions</span></span>

<span data-ttu-id="e6a6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a6f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a6f-109">Permission type</span></span>|<span data-ttu-id="e6a6f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6a6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6a6f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6a6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6a6f-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="e6a6f-112">User.Read</span></span>|
|<span data-ttu-id="e6a6f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6a6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6a6f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a6f-114">Not supported.</span></span>|
|<span data-ttu-id="e6a6f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6a6f-115">Application</span></span>|<span data-ttu-id="e6a6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6a6f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6a6f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="e6a6f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6a6f-118">Request headers</span></span>

|<span data-ttu-id="e6a6f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e6a6f-119">Name</span></span>|<span data-ttu-id="e6a6f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e6a6f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e6a6f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6a6f-121">Authorization</span></span>|<span data-ttu-id="e6a6f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6a6f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a6f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6a6f-124">Request body</span></span>

<span data-ttu-id="e6a6f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6a6f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a6f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6a6f-126">Response</span></span>

<span data-ttu-id="e6a6f-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6a6f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e6a6f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e6a6f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6a6f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6a6f-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

### <a name="response"></a><span data-ttu-id="e6a6f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6a6f-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
