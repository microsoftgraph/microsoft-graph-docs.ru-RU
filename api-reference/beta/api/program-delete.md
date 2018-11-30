---
title: Удаление программы
description: В Azure AD доступ к функции проверки, удалить объект программы.
ms.openlocfilehash: c09dcc36bfc4fbf279e7b6c49ea24bba9153c071
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080354"
---
# <a name="delete-program"></a><span data-ttu-id="93ba0-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="93ba0-103">Delete program</span></span>

> <span data-ttu-id="93ba0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93ba0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93ba0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ba0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93ba0-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD удаления объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="93ba0-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="93ba0-107">Не удаляйте программы, который по-прежнему имеет `programControl` связанных с ней рассматриваются эти доступа следует сначала удалены или не связан с программой и связано с другой программой.</span><span class="sxs-lookup"><span data-stu-id="93ba0-107">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="93ba0-108">Кроме того Обратите внимание, что программа встроенных по умолчанию удалить невозможно.</span><span class="sxs-lookup"><span data-stu-id="93ba0-108">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="93ba0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93ba0-109">Permissions</span></span>
<span data-ttu-id="93ba0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ba0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ba0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93ba0-112">Permission type</span></span>                        | <span data-ttu-id="93ba0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93ba0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93ba0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93ba0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="93ba0-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="93ba0-115"></span></span>  <span data-ttu-id="93ba0-116">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы.</span><span class="sxs-lookup"><span data-stu-id="93ba0-116">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="93ba0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93ba0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93ba0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ba0-118">Not supported.</span></span> |
|<span data-ttu-id="93ba0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93ba0-119">Application</span></span>                            | <span data-ttu-id="93ba0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ba0-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93ba0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93ba0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="93ba0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93ba0-122">Request headers</span></span>
| <span data-ttu-id="93ba0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="93ba0-123">Name</span></span>         | <span data-ttu-id="93ba0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="93ba0-124">Type</span></span>        | <span data-ttu-id="93ba0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="93ba0-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="93ba0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="93ba0-126">Authorization</span></span> | <span data-ttu-id="93ba0-127">string</span><span class="sxs-lookup"><span data-stu-id="93ba0-127">string</span></span> | <span data-ttu-id="93ba0-128">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="93ba0-128">Bearer \{token\}.</span></span> <span data-ttu-id="93ba0-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="93ba0-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93ba0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93ba0-130">Request body</span></span>
<span data-ttu-id="93ba0-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93ba0-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="93ba0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ba0-132">Response</span></span>
<span data-ttu-id="93ba0-p106">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93ba0-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93ba0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="93ba0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93ba0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="93ba0-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="93ba0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ba0-137">Response</span></span>
><span data-ttu-id="93ba0-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93ba0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
