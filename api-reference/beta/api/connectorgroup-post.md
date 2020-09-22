---
title: Создание connectorGroup
description: Создание объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d19993f8015f175c15de0de42bbfb13940c7873
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996389"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="d2168-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d2168-103">Create connectorGroup</span></span>

<span data-ttu-id="d2168-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2168-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2168-105">Создание объекта [коннекторграуп](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="d2168-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2168-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2168-106">Permissions</span></span>
<span data-ttu-id="d2168-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2168-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2168-109">Permission type</span></span>      | <span data-ttu-id="d2168-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2168-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2168-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2168-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2168-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2168-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2168-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2168-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2168-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2168-114">Not supported.</span></span>    |
|<span data-ttu-id="d2168-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2168-115">Application</span></span> | <span data-ttu-id="d2168-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2168-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d2168-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2168-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="d2168-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2168-118">Optional request headers</span></span>
| <span data-ttu-id="d2168-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2168-119">Name</span></span>       | <span data-ttu-id="d2168-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2168-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d2168-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2168-121">Authorization</span></span>  | <span data-ttu-id="d2168-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="d2168-122">Bearer.</span></span> <span data-ttu-id="d2168-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d2168-123">Required.</span></span>|
| <span data-ttu-id="d2168-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2168-124">Content-type</span></span> | <span data-ttu-id="d2168-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2168-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2168-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2168-127">Request body</span></span>
<span data-ttu-id="d2168-128">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2168-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="d2168-129">В следующей таблице перечислены свойства, доступные для **коннекторграуп**.</span><span class="sxs-lookup"><span data-stu-id="d2168-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="d2168-130">Свойство **Name** — это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="d2168-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="d2168-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2168-131">Property</span></span>     | <span data-ttu-id="d2168-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d2168-132">Type</span></span>   |<span data-ttu-id="d2168-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d2168-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2168-134">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="d2168-134">connectorGroupType</span></span>|<span data-ttu-id="d2168-135">string</span><span class="sxs-lookup"><span data-stu-id="d2168-135">string</span></span>| <span data-ttu-id="d2168-136">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="d2168-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="d2168-137">Это свойство предустановлено системой.</span><span class="sxs-lookup"><span data-stu-id="d2168-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="d2168-138">id</span><span class="sxs-lookup"><span data-stu-id="d2168-138">id</span></span>|<span data-ttu-id="d2168-139">string</span><span class="sxs-lookup"><span data-stu-id="d2168-139">string</span></span>| <span data-ttu-id="d2168-140">Уникальный идентификатор для этого Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="d2168-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="d2168-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2168-141">Read-only.</span></span> |
|<span data-ttu-id="d2168-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="d2168-142">isDefault</span></span>|<span data-ttu-id="d2168-143">boolean</span><span class="sxs-lookup"><span data-stu-id="d2168-143">boolean</span></span>| <span data-ttu-id="d2168-144">Указывает, является ли Коннекторграуп значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d2168-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="d2168-145">Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предустановлена системой.</span><span class="sxs-lookup"><span data-stu-id="d2168-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="d2168-146">name</span><span class="sxs-lookup"><span data-stu-id="d2168-146">name</span></span>|<span data-ttu-id="d2168-147">string</span><span class="sxs-lookup"><span data-stu-id="d2168-147">string</span></span>| <span data-ttu-id="d2168-148">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="d2168-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="d2168-149">региональных</span><span class="sxs-lookup"><span data-stu-id="d2168-149">region</span></span>|<span data-ttu-id="d2168-150">string</span><span class="sxs-lookup"><span data-stu-id="d2168-150">string</span></span>| <span data-ttu-id="d2168-151">Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для.</span><span class="sxs-lookup"><span data-stu-id="d2168-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="d2168-152">Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один** из соединителей или приложений.</span><span class="sxs-lookup"><span data-stu-id="d2168-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="d2168-153">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии.</span><span class="sxs-lookup"><span data-stu-id="d2168-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="d2168-154">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="d2168-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="d2168-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2168-155">Response</span></span>

<span data-ttu-id="d2168-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2168-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2168-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d2168-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2168-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2168-158">Request</span></span>
<span data-ttu-id="d2168-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2168-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2168-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2168-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
# <a name="c"></a>[<span data-ttu-id="d2168-161">C#</span><span class="sxs-lookup"><span data-stu-id="d2168-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2168-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2168-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2168-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2168-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d2168-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2168-164">Response</span></span>
<span data-ttu-id="d2168-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2168-165">The following is an example of the response.</span></span> 

><span data-ttu-id="d2168-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2168-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


