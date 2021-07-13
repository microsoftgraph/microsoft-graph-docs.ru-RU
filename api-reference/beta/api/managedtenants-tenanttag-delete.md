---
title: Удаление tenantTag
description: Удаляет объект tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e37bb368f5cd31222c1b3eaabd26fac3a5105fc7
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402645"
---
# <a name="delete-tenanttag"></a><span data-ttu-id="992a8-103">Удаление tenantTag</span><span class="sxs-lookup"><span data-stu-id="992a8-103">Delete tenantTag</span></span>
<span data-ttu-id="992a8-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="992a8-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="992a8-105">Удаляет объект [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="992a8-105">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="992a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="992a8-106">Permissions</span></span>
<span data-ttu-id="992a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="992a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="992a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="992a8-109">Permission type</span></span>|<span data-ttu-id="992a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="992a8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="992a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="992a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="992a8-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="992a8-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="992a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="992a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="992a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="992a8-114">Not supported.</span></span>|
|<span data-ttu-id="992a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="992a8-115">Application</span></span>|<span data-ttu-id="992a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="992a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="992a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="992a8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="992a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="992a8-118">Request headers</span></span>
|<span data-ttu-id="992a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="992a8-119">Name</span></span>|<span data-ttu-id="992a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="992a8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="992a8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="992a8-121">Authorization</span></span>|<span data-ttu-id="992a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="992a8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="992a8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="992a8-124">Request body</span></span>
<span data-ttu-id="992a8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="992a8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="992a8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="992a8-126">Response</span></span>

<span data-ttu-id="992a8-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="992a8-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="992a8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="992a8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="992a8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="992a8-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tenanttag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```


### <a name="response"></a><span data-ttu-id="992a8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="992a8-130">Response</span></span>
><span data-ttu-id="992a8-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="992a8-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
