---
title: Удаление программы
description: В Azure AD доступ к функции проверки, удалить объект программы.
localization_priority: Normal
ms.openlocfilehash: 930367e6c61d354655e73fb7ece9c8776e15f34e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519509"
---
# <a name="delete-program"></a><span data-ttu-id="01a4b-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="01a4b-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a4b-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD удаления объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="01a4b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="01a4b-105">Не удаляйте программы, который по-прежнему имеет `programControl` связанных с ней рассматриваются эти доступа следует сначала удалены или не связан с программой и связано с другой программой.</span><span class="sxs-lookup"><span data-stu-id="01a4b-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="01a4b-106">Кроме того Обратите внимание, что программа встроенных по умолчанию удалить невозможно.</span><span class="sxs-lookup"><span data-stu-id="01a4b-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="01a4b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01a4b-107">Permissions</span></span>
<span data-ttu-id="01a4b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01a4b-110">Permission type</span></span>                        | <span data-ttu-id="01a4b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01a4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01a4b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01a4b-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="01a4b-113"></span></span>  <span data-ttu-id="01a4b-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы.</span><span class="sxs-lookup"><span data-stu-id="01a4b-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="01a4b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01a4b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01a4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a4b-116">Not supported.</span></span> |
|<span data-ttu-id="01a4b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01a4b-117">Application</span></span>                            | <span data-ttu-id="01a4b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a4b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01a4b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01a4b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="01a4b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01a4b-120">Request headers</span></span>
| <span data-ttu-id="01a4b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="01a4b-121">Name</span></span>         | <span data-ttu-id="01a4b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="01a4b-122">Type</span></span>        | <span data-ttu-id="01a4b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="01a4b-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="01a4b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a4b-124">Authorization</span></span> | <span data-ttu-id="01a4b-125">string</span><span class="sxs-lookup"><span data-stu-id="01a4b-125">string</span></span> | <span data-ttu-id="01a4b-126">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="01a4b-126">Bearer \{token\}.</span></span> <span data-ttu-id="01a4b-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01a4b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01a4b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01a4b-128">Request body</span></span>
<span data-ttu-id="01a4b-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01a4b-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="01a4b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="01a4b-130">Response</span></span>
<span data-ttu-id="01a4b-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01a4b-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a4b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="01a4b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01a4b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="01a4b-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="01a4b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01a4b-135">Response</span></span>
><span data-ttu-id="01a4b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01a4b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
