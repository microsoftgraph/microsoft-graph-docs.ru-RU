---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a09018011e87da383371ba41b1a046ddeb9002b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577737"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="8cd31-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="8cd31-103">Delete identityProvider</span></span>

<span data-ttu-id="8cd31-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8cd31-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cd31-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd31-105">Permissions</span></span>

<span data-ttu-id="8cd31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd31-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd31-108">Permission type</span></span>      | <span data-ttu-id="8cd31-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cd31-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cd31-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cd31-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd31-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd31-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8cd31-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cd31-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8cd31-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd31-113">Not supported.</span></span>|
|<span data-ttu-id="8cd31-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cd31-114">Application</span></span>|<span data-ttu-id="8cd31-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd31-115">Not supported.</span></span>|

<span data-ttu-id="8cd31-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="8cd31-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="8cd31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cd31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8cd31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cd31-118">Request headers</span></span>

|<span data-ttu-id="8cd31-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8cd31-119">Name</span></span>|<span data-ttu-id="8cd31-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8cd31-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8cd31-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cd31-121">Authorization</span></span>|<span data-ttu-id="8cd31-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd31-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cd31-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cd31-124">Request body</span></span>

<span data-ttu-id="8cd31-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cd31-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd31-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd31-126">Response</span></span>

<span data-ttu-id="8cd31-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8cd31-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8cd31-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8cd31-128">Example</span></span>

<span data-ttu-id="8cd31-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="8cd31-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="8cd31-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cd31-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="8cd31-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd31-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
