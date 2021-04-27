---
title: Update connectorGroups
description: Обновление свойств объекта connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f4f74612ad071baae510d86c1e597bca0094c59f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047142"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="7edbe-103">Update connectorGroups</span><span class="sxs-lookup"><span data-stu-id="7edbe-103">Update connectorGroups</span></span>

<span data-ttu-id="7edbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7edbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7edbe-105">Обновление свойств объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="7edbe-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7edbe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7edbe-106">Permissions</span></span>
<span data-ttu-id="7edbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7edbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7edbe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7edbe-109">Permission type</span></span>      | <span data-ttu-id="7edbe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7edbe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7edbe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7edbe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7edbe-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7edbe-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7edbe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7edbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7edbe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7edbe-114">Not supported.</span></span>    |
|<span data-ttu-id="7edbe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7edbe-115">Application</span></span> | <span data-ttu-id="7edbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7edbe-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7edbe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7edbe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7edbe-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7edbe-118">Optional request headers</span></span>
| <span data-ttu-id="7edbe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7edbe-119">Name</span></span>       | <span data-ttu-id="7edbe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7edbe-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7edbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7edbe-121">Authorization</span></span>  | <span data-ttu-id="7edbe-122">Носителер.</span><span class="sxs-lookup"><span data-stu-id="7edbe-122">Bearer.</span></span> <span data-ttu-id="7edbe-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="7edbe-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="7edbe-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7edbe-124">Request body</span></span>
<span data-ttu-id="7edbe-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7edbe-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7edbe-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7edbe-128">Property</span></span>     | <span data-ttu-id="7edbe-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7edbe-129">Type</span></span>   |<span data-ttu-id="7edbe-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7edbe-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7edbe-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="7edbe-131">connectorGroupType</span></span>|<span data-ttu-id="7edbe-132">String</span><span class="sxs-lookup"><span data-stu-id="7edbe-132">string</span></span>| <span data-ttu-id="7edbe-133">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="7edbe-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="7edbe-134">Это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="7edbe-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="7edbe-135">id</span><span class="sxs-lookup"><span data-stu-id="7edbe-135">id</span></span>|<span data-ttu-id="7edbe-136">string</span><span class="sxs-lookup"><span data-stu-id="7edbe-136">string</span></span>| <span data-ttu-id="7edbe-137">Уникальный идентификатор для этого соединитетеляGroup.</span><span class="sxs-lookup"><span data-stu-id="7edbe-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="7edbe-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7edbe-138">Read-only.</span></span> |
|<span data-ttu-id="7edbe-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="7edbe-139">isDefault</span></span>|<span data-ttu-id="7edbe-140">boolean</span><span class="sxs-lookup"><span data-stu-id="7edbe-140">boolean</span></span>| <span data-ttu-id="7edbe-141">Указывает, является ли соединительщикОм ConnectorGroup по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7edbe-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="7edbe-142">Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="7edbe-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="7edbe-143">name</span><span class="sxs-lookup"><span data-stu-id="7edbe-143">name</span></span>|<span data-ttu-id="7edbe-144">string</span><span class="sxs-lookup"><span data-stu-id="7edbe-144">string</span></span>| <span data-ttu-id="7edbe-145">Имя, связанное с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="7edbe-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="7edbe-146">регион</span><span class="sxs-lookup"><span data-stu-id="7edbe-146">region</span></span>|<span data-ttu-id="7edbe-147">String</span><span class="sxs-lookup"><span data-stu-id="7edbe-147">string</span></span>| <span data-ttu-id="7edbe-148">Регион, в который назначен connectorGroup, и будет оптимизировать трафик.</span><span class="sxs-lookup"><span data-stu-id="7edbe-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="7edbe-149">Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе.</span><span class="sxs-lookup"><span data-stu-id="7edbe-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="7edbe-150">Доступные регионы: Северная Америка, Европа, Австралия, Азия и Индия.</span><span class="sxs-lookup"><span data-stu-id="7edbe-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="7edbe-151">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="7edbe-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="7edbe-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7edbe-152">Response</span></span>

<span data-ttu-id="7edbe-153">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект connectorGroup](../resources/connectorgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7edbe-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7edbe-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7edbe-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7edbe-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="7edbe-155">Request</span></span>
<span data-ttu-id="7edbe-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7edbe-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7edbe-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7edbe-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "region": "region-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7edbe-158">C#</span><span class="sxs-lookup"><span data-stu-id="7edbe-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7edbe-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7edbe-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7edbe-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7edbe-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7edbe-161">Java</span><span class="sxs-lookup"><span data-stu-id="7edbe-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7edbe-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7edbe-162">Response</span></span>
<span data-ttu-id="7edbe-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7edbe-163">The following is an example of the response.</span></span> <span data-ttu-id="7edbe-164">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7edbe-164">Note: The response object shown here might be shortened for readability.</span></span>
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
  "isDefault": true,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



