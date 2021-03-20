---
title: Update connectorGroups
description: Обновление свойств объекта connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9c4aadfee6674e0d363f2633c4e064ab72843551
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947071"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="3c097-103">Update connectorGroups</span><span class="sxs-lookup"><span data-stu-id="3c097-103">Update connectorGroups</span></span>

<span data-ttu-id="3c097-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c097-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c097-105">Обновление свойств объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="3c097-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c097-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c097-106">Permissions</span></span>
<span data-ttu-id="3c097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c097-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c097-109">Permission type</span></span>      | <span data-ttu-id="3c097-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c097-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c097-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c097-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c097-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c097-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c097-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c097-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c097-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c097-114">Not supported.</span></span>    |
|<span data-ttu-id="3c097-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c097-115">Application</span></span> | <span data-ttu-id="3c097-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c097-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3c097-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c097-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3c097-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c097-118">Optional request headers</span></span>
| <span data-ttu-id="3c097-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3c097-119">Name</span></span>       | <span data-ttu-id="3c097-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3c097-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3c097-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c097-121">Authorization</span></span>  | <span data-ttu-id="3c097-122">Носителер.</span><span class="sxs-lookup"><span data-stu-id="3c097-122">Bearer.</span></span> <span data-ttu-id="3c097-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3c097-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c097-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c097-124">Request body</span></span>
<span data-ttu-id="3c097-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3c097-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c097-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c097-128">Property</span></span>     | <span data-ttu-id="3c097-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3c097-129">Type</span></span>   |<span data-ttu-id="3c097-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3c097-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c097-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="3c097-131">connectorGroupType</span></span>|<span data-ttu-id="3c097-132">string</span><span class="sxs-lookup"><span data-stu-id="3c097-132">string</span></span>| <span data-ttu-id="3c097-133">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="3c097-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="3c097-134">Это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="3c097-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="3c097-135">id</span><span class="sxs-lookup"><span data-stu-id="3c097-135">id</span></span>|<span data-ttu-id="3c097-136">string</span><span class="sxs-lookup"><span data-stu-id="3c097-136">string</span></span>| <span data-ttu-id="3c097-137">Уникальный идентификатор для этого соединитетеляGroup.</span><span class="sxs-lookup"><span data-stu-id="3c097-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="3c097-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c097-138">Read-only.</span></span> |
|<span data-ttu-id="3c097-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="3c097-139">isDefault</span></span>|<span data-ttu-id="3c097-140">boolean</span><span class="sxs-lookup"><span data-stu-id="3c097-140">boolean</span></span>| <span data-ttu-id="3c097-141">Указывает, является ли соединительщикОм ConnectorGroup по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c097-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="3c097-142">Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="3c097-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="3c097-143">name</span><span class="sxs-lookup"><span data-stu-id="3c097-143">name</span></span>|<span data-ttu-id="3c097-144">string</span><span class="sxs-lookup"><span data-stu-id="3c097-144">string</span></span>| <span data-ttu-id="3c097-145">Имя, связанное с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="3c097-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="3c097-146">регион</span><span class="sxs-lookup"><span data-stu-id="3c097-146">region</span></span>|<span data-ttu-id="3c097-147">string</span><span class="sxs-lookup"><span data-stu-id="3c097-147">string</span></span>| <span data-ttu-id="3c097-148">Регион, в который назначен connectorGroup, и будет оптимизировать трафик.</span><span class="sxs-lookup"><span data-stu-id="3c097-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="3c097-149">Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе.</span><span class="sxs-lookup"><span data-stu-id="3c097-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="3c097-150">Доступные регионы: Северная Америка, Европа, Австралия, Азия и Индия.</span><span class="sxs-lookup"><span data-stu-id="3c097-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="3c097-151">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="3c097-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="3c097-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c097-152">Response</span></span>

<span data-ttu-id="3c097-153">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект connectorGroup](../resources/connectorgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c097-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c097-154">Пример</span><span class="sxs-lookup"><span data-stu-id="3c097-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c097-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c097-155">Request</span></span>
<span data-ttu-id="3c097-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c097-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c097-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c097-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c097-158">C#</span><span class="sxs-lookup"><span data-stu-id="3c097-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c097-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c097-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c097-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c097-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c097-161">Java</span><span class="sxs-lookup"><span data-stu-id="3c097-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c097-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c097-162">Response</span></span>
<span data-ttu-id="3c097-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c097-163">The following is an example of the response.</span></span> <span data-ttu-id="3c097-164">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3c097-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3c097-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c097-165">All of the properties will be returned from an actual call.</span></span>
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



