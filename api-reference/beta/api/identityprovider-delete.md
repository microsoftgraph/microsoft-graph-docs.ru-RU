---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider.
localization_priority: Normal
ms.openlocfilehash: bb64f10b656697ab2cf611dd9be0468c295b15e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501590"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="18c78-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="18c78-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18c78-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="18c78-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18c78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18c78-105">Permissions</span></span>

<span data-ttu-id="18c78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18c78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18c78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18c78-108">Permission type</span></span>      | <span data-ttu-id="18c78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18c78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18c78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18c78-110">Delegated (work or school account)</span></span>|<span data-ttu-id="18c78-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18c78-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="18c78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18c78-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="18c78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c78-113">Not supported.</span></span>|
|<span data-ttu-id="18c78-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18c78-114">Application</span></span>|<span data-ttu-id="18c78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c78-115">Not supported.</span></span>|

<span data-ttu-id="18c78-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="18c78-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="18c78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18c78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18c78-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18c78-118">Request headers</span></span>

|<span data-ttu-id="18c78-119">Имя</span><span class="sxs-lookup"><span data-stu-id="18c78-119">Name</span></span>|<span data-ttu-id="18c78-120">Описание</span><span class="sxs-lookup"><span data-stu-id="18c78-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="18c78-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18c78-121">Authorization</span></span>|<span data-ttu-id="18c78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18c78-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18c78-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18c78-124">Request body</span></span>

<span data-ttu-id="18c78-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18c78-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18c78-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="18c78-126">Response</span></span>

<span data-ttu-id="18c78-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18c78-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18c78-128">Пример</span><span class="sxs-lookup"><span data-stu-id="18c78-128">Example</span></span>

<span data-ttu-id="18c78-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="18c78-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="18c78-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18c78-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="18c78-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="18c78-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
