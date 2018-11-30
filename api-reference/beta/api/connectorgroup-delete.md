---
title: Удаление connectorGroup
description: Удалите connectorGroup.
ms.openlocfilehash: 3ba4a5a06e25f2fb1568ab9d7d6e92104ea083de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075717"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="b6f5d-103">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b6f5d-103">Delete connectorGroup</span></span>

> <span data-ttu-id="b6f5d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6f5d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6f5d-106">Удалите connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-106">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6f5d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6f5d-107">Permissions</span></span>
<span data-ttu-id="b6f5d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b6f5d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6f5d-110">Permission type</span></span>      | <span data-ttu-id="b6f5d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6f5d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f5d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6f5d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f5d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6f5d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6f5d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6f5d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-115">Not supported.</span></span>    |
|<span data-ttu-id="b6f5d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6f5d-116">Application</span></span> | <span data-ttu-id="b6f5d-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f5d-117">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b6f5d-118">**Примечание:** Соединитель группы не должно быть все соединители, связанные с ним.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-118">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="b6f5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6f5d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b6f5d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6f5d-120">Request headers</span></span>
| <span data-ttu-id="b6f5d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b6f5d-121">Name</span></span>       | <span data-ttu-id="b6f5d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b6f5d-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6f5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f5d-123">Authorization</span></span>  | <span data-ttu-id="b6f5d-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-124">Bearer.</span></span> <span data-ttu-id="b6f5d-125">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b6f5d-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f5d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6f5d-126">Request body</span></span>
<span data-ttu-id="b6f5d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f5d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f5d-128">Response</span></span>

<span data-ttu-id="b6f5d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f5d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6f5d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6f5d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6f5d-132">Request</span></span>
<span data-ttu-id="b6f5d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6f5d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="b6f5d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6f5d-134">Response</span></span>
<span data-ttu-id="b6f5d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b6f5d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
