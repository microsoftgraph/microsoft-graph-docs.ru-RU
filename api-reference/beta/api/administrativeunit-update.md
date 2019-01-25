---
title: Обновление administrativeunit
description: Обновляет свойства объекта administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3c57f8784bf642df7944bc6295ebd4fadc0ba43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511158"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="147b7-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="147b7-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="147b7-104">Обновляет свойства объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="147b7-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="147b7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="147b7-105">Permissions</span></span>
<span data-ttu-id="147b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="147b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="147b7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="147b7-108">Permission type</span></span>      | <span data-ttu-id="147b7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="147b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="147b7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="147b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="147b7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="147b7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="147b7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="147b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="147b7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="147b7-113">Not supported.</span></span>    |
|<span data-ttu-id="147b7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="147b7-114">Application</span></span> | <span data-ttu-id="147b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="147b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="147b7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="147b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="147b7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="147b7-117">Request headers</span></span>

| <span data-ttu-id="147b7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="147b7-118">Name</span></span>      |<span data-ttu-id="147b7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="147b7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="147b7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="147b7-120">Authorization</span></span>  | <span data-ttu-id="147b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="147b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="147b7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="147b7-123">Request body</span></span>

<span data-ttu-id="147b7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="147b7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="147b7-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="147b7-127">Property</span></span>   | <span data-ttu-id="147b7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="147b7-128">Type</span></span> |<span data-ttu-id="147b7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="147b7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="147b7-130">description</span><span class="sxs-lookup"><span data-stu-id="147b7-130">description</span></span>|<span data-ttu-id="147b7-131">строка</span><span class="sxs-lookup"><span data-stu-id="147b7-131">string</span></span>|<span data-ttu-id="147b7-132">Описание административных подразделения.</span><span class="sxs-lookup"><span data-stu-id="147b7-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="147b7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="147b7-133">displayName</span></span>|<span data-ttu-id="147b7-134">string</span><span class="sxs-lookup"><span data-stu-id="147b7-134">string</span></span>|<span data-ttu-id="147b7-135">Отображаемое имя для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="147b7-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="147b7-136">visibility</span><span class="sxs-lookup"><span data-stu-id="147b7-136">visibility</span></span>|<span data-ttu-id="147b7-137">string</span><span class="sxs-lookup"><span data-stu-id="147b7-137">string</span></span>|<span data-ttu-id="147b7-138">Видимость для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="147b7-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="147b7-139">Если не установлено, а затем значение по умолчанию — «общедоступный».</span><span class="sxs-lookup"><span data-stu-id="147b7-139">If not set then the default is "public".</span></span> <span data-ttu-id="147b7-140">Может иметь значение «HiddenMembership», который скрывает членство, не являющиеся членами.</span><span class="sxs-lookup"><span data-stu-id="147b7-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="147b7-141">Поскольку ресурсов **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="147b7-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="147b7-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="147b7-142">Response</span></span>

<span data-ttu-id="147b7-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="147b7-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="147b7-144">Пример</span><span class="sxs-lookup"><span data-stu-id="147b7-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="147b7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="147b7-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

##### <a name="response"></a><span data-ttu-id="147b7-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="147b7-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="147b7-147">См. также</span><span class="sxs-lookup"><span data-stu-id="147b7-147">See also</span></span>

- [<span data-ttu-id="147b7-148">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="147b7-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="147b7-149">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="147b7-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
