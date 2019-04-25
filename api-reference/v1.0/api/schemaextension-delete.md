---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 63b5f03c569439dad6615a0a23682d50646329a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521056"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="df23e-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="df23e-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df23e-104">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="df23e-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="df23e-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="df23e-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="df23e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df23e-107">Permissions</span></span>
<span data-ttu-id="df23e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df23e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df23e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df23e-110">Permission type</span></span>      | <span data-ttu-id="df23e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df23e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df23e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df23e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df23e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df23e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df23e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df23e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df23e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df23e-115">Not supported.</span></span>    |
|<span data-ttu-id="df23e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df23e-116">Application</span></span> | <span data-ttu-id="df23e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df23e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df23e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df23e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="df23e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df23e-119">Request headers</span></span>
| <span data-ttu-id="df23e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="df23e-120">Name</span></span>      |<span data-ttu-id="df23e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="df23e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df23e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df23e-122">Authorization</span></span>  | <span data-ttu-id="df23e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df23e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df23e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df23e-125">Request body</span></span>
<span data-ttu-id="df23e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df23e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df23e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="df23e-127">Response</span></span>

<span data-ttu-id="df23e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="df23e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df23e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="df23e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df23e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="df23e-131">Request</span></span>
<span data-ttu-id="df23e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df23e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="df23e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="df23e-133">Response</span></span>
<span data-ttu-id="df23e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df23e-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="df23e-135">См. также</span><span class="sxs-lookup"><span data-stu-id="df23e-135">See also</span></span>

- [<span data-ttu-id="df23e-136">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="df23e-136">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="df23e-137">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="df23e-137">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
