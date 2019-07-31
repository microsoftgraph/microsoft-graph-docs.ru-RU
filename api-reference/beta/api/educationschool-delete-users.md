---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2a09a56feb648e435ed83109c2d092ce9ada7927
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955196"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="e4b8c-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-103">Remove educationUser from an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4b8c-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4b8c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b8c-105">Permissions</span></span>

<span data-ttu-id="e4b8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4b8c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b8c-108">Permission type</span></span>                        | <span data-ttu-id="e4b8c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4b8c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e4b8c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4b8c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4b8c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-111">Not supported.</span></span>                              |
| <span data-ttu-id="e4b8c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4b8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b8c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-113">Not supported.</span></span>                              |
| <span data-ttu-id="e4b8c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4b8c-114">Application</span></span>                            | <span data-ttu-id="e4b8c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b8c-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="e4b8c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4b8c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e4b8c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4b8c-117">Request headers</span></span>

| <span data-ttu-id="e4b8c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4b8c-118">Header</span></span>        | <span data-ttu-id="e4b8c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e4b8c-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e4b8c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4b8c-120">Authorization</span></span> | <span data-ttu-id="e4b8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4b8c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4b8c-123">Request body</span></span>

<span data-ttu-id="e4b8c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4b8c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4b8c-125">Response</span></span>

<span data-ttu-id="e4b8c-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4b8c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="e4b8c-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e4b8c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4b8c-128">Request</span></span>

<span data-ttu-id="e4b8c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="e4b8c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4b8c-130">Response</span></span>

<span data-ttu-id="e4b8c-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e4b8c-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
