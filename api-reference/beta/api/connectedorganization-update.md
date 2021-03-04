---
title: Обновление объекта connectedOrganization
description: Обновление объекта connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 36619c33de483693f35c3ca1163f8e57f063622a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437417"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="4a250-103">Обновление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4a250-103">Update connectedOrganization</span></span>

<span data-ttu-id="4a250-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a250-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a250-105">[Обновим объект connectedOrganization,](../resources/connectedorganization.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="4a250-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a250-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a250-106">Permissions</span></span>
<span data-ttu-id="4a250-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a250-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a250-109">Permission type</span></span>|<span data-ttu-id="4a250-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a250-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a250-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a250-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a250-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a250-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="4a250-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a250-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a250-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a250-114">Not supported.</span></span> |
|<span data-ttu-id="4a250-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a250-115">Application</span></span>                            | <span data-ttu-id="4a250-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a250-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a250-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a250-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a250-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a250-118">Request headers</span></span>
|<span data-ttu-id="4a250-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a250-119">Name</span></span>|<span data-ttu-id="4a250-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a250-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4a250-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a250-121">Authorization</span></span>|<span data-ttu-id="4a250-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a250-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4a250-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a250-124">Content-Type</span></span>|<span data-ttu-id="4a250-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a250-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a250-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a250-127">Request body</span></span>
<span data-ttu-id="4a250-128">В теле запроса поставляем представление JSON объекта [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="4a250-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="4a250-129">В следующей таблице показаны свойства, которые можно получить при обновлении [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="4a250-129">The following table shows the properties that can be supplied when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="4a250-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a250-130">Property</span></span>|<span data-ttu-id="4a250-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a250-131">Type</span></span>|<span data-ttu-id="4a250-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a250-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="4a250-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4a250-133">displayName</span></span>  |<span data-ttu-id="4a250-134">String</span><span class="sxs-lookup"><span data-stu-id="4a250-134">String</span></span> | <span data-ttu-id="4a250-135">Имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="4a250-135">The connected organization name.</span></span>  |
| <span data-ttu-id="4a250-136">description</span><span class="sxs-lookup"><span data-stu-id="4a250-136">description</span></span>  |<span data-ttu-id="4a250-137">String</span><span class="sxs-lookup"><span data-stu-id="4a250-137">String</span></span> | <span data-ttu-id="4a250-138">Описание подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="4a250-138">The connected organization description.</span></span> |
| <span data-ttu-id="4a250-139">state</span><span class="sxs-lookup"><span data-stu-id="4a250-139">state</span></span>        |<span data-ttu-id="4a250-140">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="4a250-140">connectedOrganizationState</span></span>|<span data-ttu-id="4a250-141">Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.</span><span class="sxs-lookup"><span data-stu-id="4a250-141">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="4a250-142">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="4a250-142">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="4a250-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a250-143">Response</span></span>

<span data-ttu-id="4a250-144">В случае успешной работы этот метод возвращает код отклика и `204 Accepted` [объект connectedOrganization](../resources/connectedorganization.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a250-144">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a250-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a250-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a250-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a250-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a250-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a250-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectedorganization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization new name",
  "description":"Connected organization new description",
  "state":"configured"
}
```
# <a name="c"></a>[<span data-ttu-id="4a250-148">C#</span><span class="sxs-lookup"><span data-stu-id="4a250-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a250-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a250-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a250-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a250-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a250-151">Java</span><span class="sxs-lookup"><span data-stu-id="4a250-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4a250-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a250-152">Response</span></span>
<span data-ttu-id="4a250-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a250-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 204 Accepted
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization new name",
  "description":"Connected organization new description",
  "state":"configured"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


