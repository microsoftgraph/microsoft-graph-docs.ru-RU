---
title: Обновление объекта Коннектедорганизатион
description: Обновление объекта Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f7591a709065e42e9de87ea94873454512bbb0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996481"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="163df-103">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="163df-103">Update connectedOrganization</span></span>

<span data-ttu-id="163df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="163df-105">Обновление объекта [коннектедорганизатион](../resources/connectedorganization.md) для изменения одного или нескольких его свойств.</span><span class="sxs-lookup"><span data-stu-id="163df-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="163df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="163df-106">Permissions</span></span>
<span data-ttu-id="163df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="163df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="163df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="163df-109">Permission type</span></span>|<span data-ttu-id="163df-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="163df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="163df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="163df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="163df-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="163df-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="163df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="163df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="163df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="163df-114">Not supported.</span></span> |
|<span data-ttu-id="163df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="163df-115">Application</span></span>                            | <span data-ttu-id="163df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="163df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="163df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="163df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="163df-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="163df-118">Request headers</span></span>
|<span data-ttu-id="163df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="163df-119">Name</span></span>|<span data-ttu-id="163df-120">Описание</span><span class="sxs-lookup"><span data-stu-id="163df-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="163df-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="163df-121">Authorization</span></span>|<span data-ttu-id="163df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="163df-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="163df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="163df-124">Content-Type</span></span>|<span data-ttu-id="163df-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="163df-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="163df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="163df-127">Request body</span></span>
<span data-ttu-id="163df-128">В тексте запроса добавьте представление объекта [коннектедорганизатион](../resources/connectedorganization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="163df-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="163df-129">В следующей таблице приведены свойства, необходимые при обновлении [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="163df-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="163df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="163df-130">Property</span></span>|<span data-ttu-id="163df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="163df-131">Type</span></span>|<span data-ttu-id="163df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="163df-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="163df-133">displayName</span><span class="sxs-lookup"><span data-stu-id="163df-133">displayName</span></span>  |<span data-ttu-id="163df-134">String</span><span class="sxs-lookup"><span data-stu-id="163df-134">String</span></span> | <span data-ttu-id="163df-135">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="163df-135">The connected organization name.</span></span>  |
| <span data-ttu-id="163df-136">description</span><span class="sxs-lookup"><span data-stu-id="163df-136">description</span></span>  |<span data-ttu-id="163df-137">String</span><span class="sxs-lookup"><span data-stu-id="163df-137">String</span></span> | <span data-ttu-id="163df-138">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="163df-138">The connected organization description.</span></span> |
| <span data-ttu-id="163df-139">state</span><span class="sxs-lookup"><span data-stu-id="163df-139">state</span></span>        |<span data-ttu-id="163df-140">коннектедорганизатионстате</span><span class="sxs-lookup"><span data-stu-id="163df-140">connectedOrganizationState</span></span>|<span data-ttu-id="163df-141">Состояние подключенной Организации определяет, применимы ли политики назначения с типом области запрашивающего `AllConfiguredConnectedOrganizationSubjects` .</span><span class="sxs-lookup"><span data-stu-id="163df-141">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="163df-142">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="163df-142">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="163df-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="163df-143">Response</span></span>

<span data-ttu-id="163df-144">В случае успешного выполнения этот метод возвращает `204 Accepted` код отклика и объект [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="163df-144">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="163df-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="163df-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="163df-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="163df-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="163df-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="163df-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="163df-148">C#</span><span class="sxs-lookup"><span data-stu-id="163df-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="163df-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="163df-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="163df-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="163df-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="163df-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="163df-151">Response</span></span>
<span data-ttu-id="163df-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="163df-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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


