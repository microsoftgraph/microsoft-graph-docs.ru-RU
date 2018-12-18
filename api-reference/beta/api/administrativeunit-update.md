---
title: Обновление administrativeunit
description: Обновляет свойства объекта administrativeUnit.
author: lleonard-msft
ms.openlocfilehash: 99ec27bc9a60e25d28202d2ebd82155089963c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362169"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="9dead-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="9dead-103">Update administrativeunit</span></span>

> <span data-ttu-id="9dead-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9dead-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dead-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dead-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9dead-106">Обновляет свойства объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="9dead-106">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9dead-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dead-107">Permissions</span></span>
<span data-ttu-id="9dead-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dead-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9dead-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dead-110">Permission type</span></span>      | <span data-ttu-id="9dead-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dead-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dead-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dead-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9dead-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9dead-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9dead-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dead-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dead-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dead-115">Not supported.</span></span>    |
|<span data-ttu-id="9dead-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dead-116">Application</span></span> | <span data-ttu-id="9dead-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dead-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dead-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dead-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9dead-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dead-119">Request headers</span></span>

| <span data-ttu-id="9dead-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9dead-120">Name</span></span>      |<span data-ttu-id="9dead-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9dead-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9dead-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dead-122">Authorization</span></span>  | <span data-ttu-id="9dead-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dead-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dead-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dead-125">Request body</span></span>

<span data-ttu-id="9dead-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9dead-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9dead-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dead-129">Property</span></span>   | <span data-ttu-id="9dead-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9dead-130">Type</span></span> |<span data-ttu-id="9dead-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9dead-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dead-132">description</span><span class="sxs-lookup"><span data-stu-id="9dead-132">description</span></span>|<span data-ttu-id="9dead-133">строка</span><span class="sxs-lookup"><span data-stu-id="9dead-133">string</span></span>|<span data-ttu-id="9dead-134">Описание административных подразделения.</span><span class="sxs-lookup"><span data-stu-id="9dead-134">Description for the administrative unit.</span></span>|
|<span data-ttu-id="9dead-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9dead-135">displayName</span></span>|<span data-ttu-id="9dead-136">строка</span><span class="sxs-lookup"><span data-stu-id="9dead-136">string</span></span>|<span data-ttu-id="9dead-137">Отображаемое имя для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="9dead-137">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="9dead-138">visibility</span><span class="sxs-lookup"><span data-stu-id="9dead-138">visibility</span></span>|<span data-ttu-id="9dead-139">string</span><span class="sxs-lookup"><span data-stu-id="9dead-139">string</span></span>|<span data-ttu-id="9dead-140">Видимость для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="9dead-140">Visibility for the administrative unit.</span></span> <span data-ttu-id="9dead-141">Если не установлено, а затем значение по умолчанию — «общедоступный».</span><span class="sxs-lookup"><span data-stu-id="9dead-141">If not set then the default is "public".</span></span> <span data-ttu-id="9dead-142">Может иметь значение «HiddenMembership», который скрывает членство, не являющиеся членами.</span><span class="sxs-lookup"><span data-stu-id="9dead-142">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="9dead-143">Поскольку ресурсов **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="9dead-143">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="9dead-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dead-144">Response</span></span>

<span data-ttu-id="9dead-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9dead-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9dead-146">Пример</span><span class="sxs-lookup"><span data-stu-id="9dead-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9dead-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dead-147">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="9dead-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dead-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9dead-149">См. также</span><span class="sxs-lookup"><span data-stu-id="9dead-149">See also</span></span>

- [<span data-ttu-id="9dead-150">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9dead-150">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9dead-151">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9dead-151">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->