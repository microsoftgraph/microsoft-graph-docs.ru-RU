---
title: Удаление identityProvider
description: Удаление существующих identityProvider.
localization_priority: Normal
ms.openlocfilehash: bb64f10b656697ab2cf611dd9be0468c295b15e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514357"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="3955a-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="3955a-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3955a-104">Удаление существующих [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="3955a-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3955a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3955a-105">Permissions</span></span>

<span data-ttu-id="3955a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3955a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3955a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3955a-108">Permission type</span></span>      | <span data-ttu-id="3955a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3955a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3955a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3955a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3955a-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3955a-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3955a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3955a-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3955a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3955a-113">Not supported.</span></span>|
|<span data-ttu-id="3955a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3955a-114">Application</span></span>|<span data-ttu-id="3955a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3955a-115">Not supported.</span></span>|

<span data-ttu-id="3955a-116">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="3955a-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3955a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3955a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3955a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3955a-118">Request headers</span></span>

|<span data-ttu-id="3955a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3955a-119">Name</span></span>|<span data-ttu-id="3955a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3955a-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3955a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3955a-121">Authorization</span></span>|<span data-ttu-id="3955a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3955a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3955a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3955a-124">Request body</span></span>

<span data-ttu-id="3955a-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3955a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3955a-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="3955a-126">Response</span></span>

<span data-ttu-id="3955a-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3955a-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3955a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3955a-128">Example</span></span>

<span data-ttu-id="3955a-129">В следующем примере удаляется **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="3955a-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="3955a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3955a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="3955a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3955a-131">Response</span></span>

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
