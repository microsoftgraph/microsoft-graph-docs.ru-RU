---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного ресурса schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: cdd0ac41e65e72ba16f5111c8b67869321f934dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938498"
---
# <a name="update-schemaextension"></a><span data-ttu-id="4d639-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="4d639-103">Update schemaExtension</span></span>

> <span data-ttu-id="4d639-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d639-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d639-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d639-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d639-106">Обновление свойств в определении указанного ресурса [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="4d639-106">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="4d639-p102">Это обновление применяется ко всем ресурсам, включенным в свойство **targetTypes** расширения. Эти ресурсы входят в число [поддерживаемых](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="4d639-p102">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="4d639-p103">Только приложение, которое создало расширение схемы (приложение-владелец), может внести дополнения в расширение, причем только тогда, когда расширение находится в состоянии **InDevelopment** или **Available**. Это означает, что приложению не удастся удалить настраиваемые свойства или целевые типы ресурсов из определения. Но приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="4d639-p103">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d639-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d639-112">Permissions</span></span>

<span data-ttu-id="4d639-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d639-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d639-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d639-115">Permission type</span></span>      | <span data-ttu-id="4d639-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d639-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d639-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d639-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4d639-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d639-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d639-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d639-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d639-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d639-120">Not supported.</span></span>    |
|<span data-ttu-id="4d639-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d639-121">Application</span></span> | <span data-ttu-id="4d639-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d639-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d639-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d639-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4d639-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d639-124">Optional request headers</span></span>

| <span data-ttu-id="4d639-125">Имя</span><span class="sxs-lookup"><span data-stu-id="4d639-125">Name</span></span>      |<span data-ttu-id="4d639-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4d639-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d639-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d639-127">Authorization</span></span>  | <span data-ttu-id="4d639-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d639-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d639-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d639-130">Content-Type</span></span>   | <span data-ttu-id="4d639-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4d639-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d639-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d639-132">Request body</span></span>

<span data-ttu-id="4d639-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4d639-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4d639-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d639-136">Property</span></span>   | <span data-ttu-id="4d639-137">Тип</span><span class="sxs-lookup"><span data-stu-id="4d639-137">Type</span></span> |<span data-ttu-id="4d639-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4d639-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d639-139">описание</span><span class="sxs-lookup"><span data-stu-id="4d639-139">description</span></span>|<span data-ttu-id="4d639-140">String</span><span class="sxs-lookup"><span data-stu-id="4d639-140">String</span></span>|<span data-ttu-id="4d639-141">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="4d639-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="4d639-142">свойства</span><span class="sxs-lookup"><span data-stu-id="4d639-142">properties</span></span>|<span data-ttu-id="4d639-143">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4d639-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="4d639-p107">Коллекция имен и типов свойств, составляющих определение расширения схемы. Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="4d639-p107">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="4d639-146">status</span><span class="sxs-lookup"><span data-stu-id="4d639-146">status</span></span>|<span data-ttu-id="4d639-147">String</span><span class="sxs-lookup"><span data-stu-id="4d639-147">String</span></span>|<span data-ttu-id="4d639-148">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="4d639-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="4d639-149">Начальное состояние после создания — **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="4d639-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="4d639-150">Смены состояний: от **InDevelopment** **доступен** и **доступен** для **устарел**.</span><span class="sxs-lookup"><span data-stu-id="4d639-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="4d639-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="4d639-151">targetTypes</span></span>|<span data-ttu-id="4d639-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4d639-152">String collection</span></span>|<span data-ttu-id="4d639-p109">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="4d639-p109">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="4d639-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d639-155">Response</span></span>

<span data-ttu-id="4d639-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d639-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d639-157">Пример</span><span class="sxs-lookup"><span data-stu-id="4d639-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d639-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d639-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="4d639-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d639-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4d639-160">См. также</span><span class="sxs-lookup"><span data-stu-id="4d639-160">See also</span></span>

- [<span data-ttu-id="4d639-161">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4d639-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4d639-162">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="4d639-162">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
