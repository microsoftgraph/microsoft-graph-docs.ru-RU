---
title: Создание connectorGroup
description: Создание объекта connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 188bb45cc664681cf536617a77072a0bb409f755
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947088"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="66b54-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="66b54-103">Create connectorGroup</span></span>

<span data-ttu-id="66b54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66b54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66b54-105">Создание объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="66b54-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66b54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66b54-106">Permissions</span></span>
<span data-ttu-id="66b54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66b54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66b54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66b54-109">Permission type</span></span>      | <span data-ttu-id="66b54-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66b54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66b54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66b54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66b54-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66b54-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66b54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66b54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66b54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b54-114">Not supported.</span></span>    |
|<span data-ttu-id="66b54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66b54-115">Application</span></span> | <span data-ttu-id="66b54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b54-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="66b54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66b54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="66b54-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66b54-118">Optional request headers</span></span>
| <span data-ttu-id="66b54-119">Имя</span><span class="sxs-lookup"><span data-stu-id="66b54-119">Name</span></span>       | <span data-ttu-id="66b54-120">Описание</span><span class="sxs-lookup"><span data-stu-id="66b54-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="66b54-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b54-121">Authorization</span></span>  | <span data-ttu-id="66b54-122">Носителер.</span><span class="sxs-lookup"><span data-stu-id="66b54-122">Bearer.</span></span> <span data-ttu-id="66b54-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="66b54-123">Required.</span></span>|
| <span data-ttu-id="66b54-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66b54-124">Content-type</span></span> | <span data-ttu-id="66b54-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66b54-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66b54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66b54-127">Request body</span></span>
<span data-ttu-id="66b54-128">В теле запроса поставляем представление JSON объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="66b54-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="66b54-129">В следующей таблице перечислены свойства, доступные для **connectorGroup.**</span><span class="sxs-lookup"><span data-stu-id="66b54-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="66b54-130">Свойство **name** — обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="66b54-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="66b54-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="66b54-131">Property</span></span>     | <span data-ttu-id="66b54-132">Тип</span><span class="sxs-lookup"><span data-stu-id="66b54-132">Type</span></span>   |<span data-ttu-id="66b54-133">Описание</span><span class="sxs-lookup"><span data-stu-id="66b54-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66b54-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="66b54-134">connectorGroupType</span></span>|<span data-ttu-id="66b54-135">string</span><span class="sxs-lookup"><span data-stu-id="66b54-135">string</span></span>| <span data-ttu-id="66b54-136">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="66b54-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="66b54-137">Это свойство заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="66b54-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="66b54-138">id</span><span class="sxs-lookup"><span data-stu-id="66b54-138">id</span></span>|<span data-ttu-id="66b54-139">string</span><span class="sxs-lookup"><span data-stu-id="66b54-139">string</span></span>| <span data-ttu-id="66b54-140">Уникальный идентификатор для этого соединитетеляGroup.</span><span class="sxs-lookup"><span data-stu-id="66b54-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="66b54-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66b54-141">Read-only.</span></span> |
|<span data-ttu-id="66b54-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="66b54-142">isDefault</span></span>|<span data-ttu-id="66b54-143">boolean</span><span class="sxs-lookup"><span data-stu-id="66b54-143">boolean</span></span>| <span data-ttu-id="66b54-144">Указывает, является ли соединительщикGroup по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="66b54-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="66b54-145">Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой.</span><span class="sxs-lookup"><span data-stu-id="66b54-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="66b54-146">name</span><span class="sxs-lookup"><span data-stu-id="66b54-146">name</span></span>|<span data-ttu-id="66b54-147">string</span><span class="sxs-lookup"><span data-stu-id="66b54-147">string</span></span>| <span data-ttu-id="66b54-148">Имя, связанное с соединитетелемGroup.</span><span class="sxs-lookup"><span data-stu-id="66b54-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="66b54-149">регион</span><span class="sxs-lookup"><span data-stu-id="66b54-149">region</span></span>|<span data-ttu-id="66b54-150">string</span><span class="sxs-lookup"><span data-stu-id="66b54-150">string</span></span>| <span data-ttu-id="66b54-151">Регион, в который назначен connectorGroup, и будет оптимизировать трафик.</span><span class="sxs-lookup"><span data-stu-id="66b54-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="66b54-152">Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе.</span><span class="sxs-lookup"><span data-stu-id="66b54-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="66b54-153">Доступные регионы: Северная Америка, Европа, Австралия, Азия и Индия.</span><span class="sxs-lookup"><span data-stu-id="66b54-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="66b54-154">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="66b54-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="66b54-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b54-155">Response</span></span>

<span data-ttu-id="66b54-156">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [connectorGroup](../resources/connectorgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="66b54-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66b54-157">Пример</span><span class="sxs-lookup"><span data-stu-id="66b54-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="66b54-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="66b54-158">Request</span></span>
<span data-ttu-id="66b54-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66b54-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66b54-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="66b54-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup_1"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
# <a name="c"></a>[<span data-ttu-id="66b54-161">C#</span><span class="sxs-lookup"><span data-stu-id="66b54-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66b54-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66b54-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66b54-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66b54-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66b54-164">Java</span><span class="sxs-lookup"><span data-stu-id="66b54-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="66b54-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b54-165">Response</span></span>
<span data-ttu-id="66b54-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66b54-166">The following is an example of the response.</span></span> 

><span data-ttu-id="66b54-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66b54-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



