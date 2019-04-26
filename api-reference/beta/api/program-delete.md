---
title: Удаление программы
description: В функции рецензирования Access Azure AD удалите объект Program.
localization_priority: Normal
ms.openlocfilehash: e3839c552d7342bc00f5fdf8c26d45770c12ff17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331987"
---
# <a name="delete-program"></a><span data-ttu-id="a344a-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="a344a-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a344a-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="a344a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="a344a-105">Не удаляйте программу, с которой все `programControl` еще связаны, эти проверки доступа сначала необходимо удалить или удалить из программы, а затем связать с другой программой.</span><span class="sxs-lookup"><span data-stu-id="a344a-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="a344a-106">Кроме того, обратите внимание на то, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="a344a-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="a344a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a344a-107">Permissions</span></span>
<span data-ttu-id="a344a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a344a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a344a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a344a-110">Permission type</span></span>                        | <span data-ttu-id="a344a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a344a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a344a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a344a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a344a-113">Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a344a-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="a344a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a344a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a344a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a344a-115">Not supported.</span></span> |
|<span data-ttu-id="a344a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a344a-116">Application</span></span>                            | <span data-ttu-id="a344a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a344a-117">Not supported.</span></span> |

<span data-ttu-id="a344a-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="a344a-118">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="a344a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a344a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="a344a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a344a-120">Request headers</span></span>
| <span data-ttu-id="a344a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a344a-121">Name</span></span>         | <span data-ttu-id="a344a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a344a-122">Type</span></span>        | <span data-ttu-id="a344a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a344a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a344a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a344a-124">Authorization</span></span> | <span data-ttu-id="a344a-125">string</span><span class="sxs-lookup"><span data-stu-id="a344a-125">string</span></span> | <span data-ttu-id="a344a-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a344a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a344a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a344a-128">Request body</span></span>
<span data-ttu-id="a344a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a344a-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a344a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a344a-130">Response</span></span>
<span data-ttu-id="a344a-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a344a-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a344a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a344a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a344a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a344a-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="a344a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a344a-135">Response</span></span>
><span data-ttu-id="a344a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a344a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
