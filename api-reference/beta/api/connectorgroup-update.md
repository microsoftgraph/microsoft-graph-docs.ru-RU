---
title: Обновление connectorGroups
description: Обновление свойства объекта connectorgroup.
ms.openlocfilehash: a9777394a3ecfc65a7c03c07643359ef3c763aca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075040"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="03e84-103">Обновление connectorGroups</span><span class="sxs-lookup"><span data-stu-id="03e84-103">Update connectorGroups</span></span>

> <span data-ttu-id="03e84-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03e84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03e84-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e84-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03e84-106">Обновление свойства объекта connectorgroup.</span><span class="sxs-lookup"><span data-stu-id="03e84-106">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="03e84-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03e84-107">Permissions</span></span>
<span data-ttu-id="03e84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03e84-110">Permission type</span></span>      | <span data-ttu-id="03e84-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03e84-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03e84-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03e84-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03e84-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03e84-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03e84-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e84-115">Not supported.</span></span>    |
|<span data-ttu-id="03e84-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03e84-116">Application</span></span> | <span data-ttu-id="03e84-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e84-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e84-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03e84-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="03e84-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03e84-119">Optional request headers</span></span>
| <span data-ttu-id="03e84-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03e84-120">Name</span></span>       | <span data-ttu-id="03e84-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03e84-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03e84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03e84-122">Authorization</span></span>  | <span data-ttu-id="03e84-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="03e84-123">Bearer.</span></span> <span data-ttu-id="03e84-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="03e84-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e84-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03e84-125">Request body</span></span>
<span data-ttu-id="03e84-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="03e84-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03e84-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="03e84-129">Property</span></span>     | <span data-ttu-id="03e84-130">Тип</span><span class="sxs-lookup"><span data-stu-id="03e84-130">Type</span></span>   |<span data-ttu-id="03e84-131">Description</span><span class="sxs-lookup"><span data-stu-id="03e84-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e84-132">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="03e84-132">connectorGroupType</span></span>|<span data-ttu-id="03e84-133">string</span><span class="sxs-lookup"><span data-stu-id="03e84-133">string</span></span>| <span data-ttu-id="03e84-134">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="03e84-134">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="03e84-135">name</span><span class="sxs-lookup"><span data-stu-id="03e84-135">name</span></span>|<span data-ttu-id="03e84-136">String</span><span class="sxs-lookup"><span data-stu-id="03e84-136">String</span></span>|<span data-ttu-id="03e84-137">Имя connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="03e84-137">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="03e84-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="03e84-138">Response</span></span>

<span data-ttu-id="03e84-139">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [connectorGroup](../resources/connectorgroup.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03e84-139">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03e84-140">Пример</span><span class="sxs-lookup"><span data-stu-id="03e84-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03e84-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="03e84-141">Request</span></span>
<span data-ttu-id="03e84-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03e84-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="03e84-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="03e84-143">Response</span></span>
<span data-ttu-id="03e84-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="03e84-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
