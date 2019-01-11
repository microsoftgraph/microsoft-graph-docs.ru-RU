---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
ms.openlocfilehash: 8641b00b984380592f14ae366b9cc20ab11dc7b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842198"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="b0acd-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b0acd-103">Delete schemaExtension</span></span>

> <span data-ttu-id="b0acd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0acd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0acd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0acd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0acd-106">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="b0acd-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="b0acd-p102">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="b0acd-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="b0acd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0acd-109">Permissions</span></span>
<span data-ttu-id="b0acd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0acd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0acd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0acd-112">Permission type</span></span>      | <span data-ttu-id="b0acd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0acd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0acd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0acd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b0acd-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0acd-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0acd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0acd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0acd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0acd-117">Not supported.</span></span>    |
|<span data-ttu-id="b0acd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0acd-118">Application</span></span> | <span data-ttu-id="b0acd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0acd-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0acd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0acd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0acd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0acd-121">Request headers</span></span>
| <span data-ttu-id="b0acd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b0acd-122">Name</span></span>      |<span data-ttu-id="b0acd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b0acd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0acd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0acd-124">Authorization</span></span>  | <span data-ttu-id="b0acd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0acd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0acd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0acd-127">Request body</span></span>
<span data-ttu-id="b0acd-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0acd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0acd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0acd-129">Response</span></span>

<span data-ttu-id="b0acd-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b0acd-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0acd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0acd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0acd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0acd-133">Request</span></span>
<span data-ttu-id="b0acd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0acd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="b0acd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0acd-135">Response</span></span>
<span data-ttu-id="b0acd-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0acd-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b0acd-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b0acd-137">See also</span></span>

- [<span data-ttu-id="b0acd-138">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b0acd-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b0acd-139">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="b0acd-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
