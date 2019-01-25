---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного ресурса schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515540"
---
# <a name="update-schemaextension"></a><span data-ttu-id="fa1a9-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="fa1a9-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa1a9-104">Обновление свойств в определении указанного ресурса [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="fa1a9-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="fa1a9-p101">Это обновление применяется ко всем ресурсам, включенным в свойство **targetTypes** расширения. Эти ресурсы входят в число [поддерживаемых](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="fa1a9-p102">Только приложение, которое создало расширение схемы (приложение-владелец), может внести дополнения в расширение, причем только тогда, когда расширение находится в состоянии **InDevelopment** или **Available**. Это означает, что приложению не удастся удалить настраиваемые свойства или целевые типы ресурсов из определения. Но приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa1a9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1a9-110">Permissions</span></span>

<span data-ttu-id="fa1a9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa1a9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1a9-113">Permission type</span></span>      | <span data-ttu-id="fa1a9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa1a9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa1a9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa1a9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fa1a9-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa1a9-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa1a9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa1a9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa1a9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-118">Not supported.</span></span>    |
|<span data-ttu-id="fa1a9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa1a9-119">Application</span></span> | <span data-ttu-id="fa1a9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa1a9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa1a9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fa1a9-122">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa1a9-122">Optional request headers</span></span>

| <span data-ttu-id="fa1a9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fa1a9-123">Name</span></span>      |<span data-ttu-id="fa1a9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fa1a9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa1a9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa1a9-125">Authorization</span></span>  | <span data-ttu-id="fa1a9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa1a9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa1a9-128">Content-Type</span></span>   | <span data-ttu-id="fa1a9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fa1a9-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa1a9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa1a9-130">Request body</span></span>

<span data-ttu-id="fa1a9-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa1a9-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa1a9-134">Property</span></span>   | <span data-ttu-id="fa1a9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="fa1a9-135">Type</span></span> |<span data-ttu-id="fa1a9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fa1a9-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa1a9-137">description</span><span class="sxs-lookup"><span data-stu-id="fa1a9-137">description</span></span>|<span data-ttu-id="fa1a9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fa1a9-138">String</span></span>|<span data-ttu-id="fa1a9-139">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="fa1a9-140">properties</span><span class="sxs-lookup"><span data-stu-id="fa1a9-140">properties</span></span>|<span data-ttu-id="fa1a9-141">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="fa1a9-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="fa1a9-p106">Коллекция имен и типов свойств, составляющих определение расширения схемы. Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="fa1a9-144">status</span><span class="sxs-lookup"><span data-stu-id="fa1a9-144">status</span></span>|<span data-ttu-id="fa1a9-145">String</span><span class="sxs-lookup"><span data-stu-id="fa1a9-145">String</span></span>|<span data-ttu-id="fa1a9-146">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="fa1a9-147">Начальное состояние после создания — **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="fa1a9-148">Смены состояний: от **InDevelopment** **доступен** и **доступен** для **устарел**.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="fa1a9-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="fa1a9-149">targetTypes</span></span>|<span data-ttu-id="fa1a9-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa1a9-150">String collection</span></span>|<span data-ttu-id="fa1a9-p108">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="fa1a9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa1a9-153">Response</span></span>

<span data-ttu-id="fa1a9-154">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fa1a9-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa1a9-155">Пример</span><span class="sxs-lookup"><span data-stu-id="fa1a9-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa1a9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa1a9-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="fa1a9-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa1a9-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="fa1a9-158">См. также</span><span class="sxs-lookup"><span data-stu-id="fa1a9-158">See also</span></span>

- [<span data-ttu-id="fa1a9-159">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fa1a9-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fa1a9-160">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="fa1a9-160">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
