---
title: Список identityProviders
description: Извлечение всех identityProviders в каталоге.
localization_priority: Normal
ms.openlocfilehash: 4226e6f091527d2df8bfb544327ec2e49f2b890c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529735"
---
# <a name="list-identityproviders"></a><span data-ttu-id="e47ce-103">Список identityProviders</span><span class="sxs-lookup"><span data-stu-id="e47ce-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e47ce-104">Извлечение всех [identityProviders](../resources/identityprovider.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="e47ce-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="e47ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e47ce-105">Permissions</span></span>

<span data-ttu-id="e47ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e47ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e47ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e47ce-108">Permission type</span></span>      | <span data-ttu-id="e47ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e47ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e47ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e47ce-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e47ce-111">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ce-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e47ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e47ce-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e47ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e47ce-113">Not supported.</span></span>|
|<span data-ttu-id="e47ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e47ce-114">Application</span></span>|<span data-ttu-id="e47ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e47ce-115">Not supported.</span></span>|

<span data-ttu-id="e47ce-116">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="e47ce-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e47ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e47ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e47ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e47ce-118">Request headers</span></span>

|<span data-ttu-id="e47ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e47ce-119">Name</span></span>|<span data-ttu-id="e47ce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e47ce-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e47ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e47ce-121">Authorization</span></span>|<span data-ttu-id="e47ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e47ce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e47ce-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e47ce-124">Request body</span></span>

<span data-ttu-id="e47ce-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e47ce-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e47ce-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="e47ce-126">Response</span></span>

<span data-ttu-id="e47ce-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию [identityProviders](../resources/identityprovider.md) в представление JSON в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e47ce-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e47ce-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e47ce-128">Example</span></span>

<span data-ttu-id="e47ce-129">В следующем примере извлекаются все **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e47ce-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e47ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e47ce-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="e47ce-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e47ce-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
