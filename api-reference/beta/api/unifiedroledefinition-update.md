---
title: Обновление Унифиедроледефинитион
description: Обновление свойств объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee564c893473231cddf68e804b767c2f8142137a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452057"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="39dbe-103">Обновление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="39dbe-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="39dbe-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="39dbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39dbe-105">Обновление свойств объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="39dbe-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39dbe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39dbe-106">Permissions</span></span>

<span data-ttu-id="39dbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39dbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39dbe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39dbe-109">Permission type</span></span>                        | <span data-ttu-id="39dbe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39dbe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39dbe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39dbe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39dbe-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="39dbe-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="39dbe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39dbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39dbe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39dbe-114">Not supported.</span></span> |
| <span data-ttu-id="39dbe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39dbe-115">Application</span></span>                            | <span data-ttu-id="39dbe-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="39dbe-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="39dbe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39dbe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39dbe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39dbe-118">Request headers</span></span>

| <span data-ttu-id="39dbe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39dbe-119">Name</span></span>       | <span data-ttu-id="39dbe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39dbe-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39dbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39dbe-121">Authorization</span></span> | <span data-ttu-id="39dbe-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="39dbe-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="39dbe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39dbe-123">Request body</span></span>

<span data-ttu-id="39dbe-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="39dbe-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="39dbe-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="39dbe-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="39dbe-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="39dbe-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39dbe-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="39dbe-127">Property</span></span>     | <span data-ttu-id="39dbe-128">Тип</span><span class="sxs-lookup"><span data-stu-id="39dbe-128">Type</span></span>        | <span data-ttu-id="39dbe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="39dbe-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39dbe-130">description</span><span class="sxs-lookup"><span data-stu-id="39dbe-130">description</span></span>|<span data-ttu-id="39dbe-131">String</span><span class="sxs-lookup"><span data-stu-id="39dbe-131">String</span></span>| <span data-ttu-id="39dbe-132">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="39dbe-132">The description for the role definition.</span></span> <span data-ttu-id="39dbe-133">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="39dbe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="39dbe-134">displayName</span></span>|<span data-ttu-id="39dbe-135">Строка</span><span class="sxs-lookup"><span data-stu-id="39dbe-135">String</span></span>| <span data-ttu-id="39dbe-136">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="39dbe-136">The display name for the role definition.</span></span> <span data-ttu-id="39dbe-137">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="39dbe-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39dbe-138">Required.</span></span>|
|<span data-ttu-id="39dbe-139">id</span><span class="sxs-lookup"><span data-stu-id="39dbe-139">id</span></span>|<span data-ttu-id="39dbe-140">String</span><span class="sxs-lookup"><span data-stu-id="39dbe-140">String</span></span>| <span data-ttu-id="39dbe-141">Уникальный идентификатор для определения роли.</span><span class="sxs-lookup"><span data-stu-id="39dbe-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="39dbe-142">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39dbe-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="39dbe-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="39dbe-143">isBuiltIn</span></span>|<span data-ttu-id="39dbe-144">Логический</span><span class="sxs-lookup"><span data-stu-id="39dbe-144">Boolean</span></span>| <span data-ttu-id="39dbe-145">Флаг, указывающий, является ли определение роли частью набора по умолчанию, входящего в состав продукта или настраиваемого.</span><span class="sxs-lookup"><span data-stu-id="39dbe-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="39dbe-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39dbe-146">Read-only.</span></span> |
|<span data-ttu-id="39dbe-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="39dbe-147">isEnabled</span></span>|<span data-ttu-id="39dbe-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="39dbe-148">Boolean</span></span>| <span data-ttu-id="39dbe-149">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="39dbe-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="39dbe-150">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="39dbe-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="39dbe-151">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="39dbe-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="39dbe-152">resourceScopes</span></span>|<span data-ttu-id="39dbe-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39dbe-153">String collection</span></span>| <span data-ttu-id="39dbe-154">Список разрешений областей, к которым применяется определение роли.</span><span class="sxs-lookup"><span data-stu-id="39dbe-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="39dbe-155">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="39dbe-155">Currently only "/" is supported.</span></span> <span data-ttu-id="39dbe-156">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-156">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="39dbe-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="39dbe-157">rolePermissions</span></span>|<span data-ttu-id="39dbe-158">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="39dbe-158">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="39dbe-159">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="39dbe-159">List of permissions included in the role.</span></span> <span data-ttu-id="39dbe-160">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-160">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="39dbe-161">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="39dbe-161">Required.</span></span> |
|<span data-ttu-id="39dbe-162">templateId</span><span class="sxs-lookup"><span data-stu-id="39dbe-162">templateId</span></span>|<span data-ttu-id="39dbe-163">String</span><span class="sxs-lookup"><span data-stu-id="39dbe-163">String</span></span>| <span data-ttu-id="39dbe-164">Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false.</span><span class="sxs-lookup"><span data-stu-id="39dbe-164">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="39dbe-165">Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов.</span><span class="sxs-lookup"><span data-stu-id="39dbe-165">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="39dbe-166">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-166">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="39dbe-167">version</span><span class="sxs-lookup"><span data-stu-id="39dbe-167">version</span></span>|<span data-ttu-id="39dbe-168">String</span><span class="sxs-lookup"><span data-stu-id="39dbe-168">String</span></span>| <span data-ttu-id="39dbe-169">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="39dbe-169">Indicates version of the role definition.</span></span> <span data-ttu-id="39dbe-170">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="39dbe-170">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="39dbe-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dbe-171">Response</span></span>

<span data-ttu-id="39dbe-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39dbe-172">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39dbe-173">Пример</span><span class="sxs-lookup"><span data-stu-id="39dbe-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="39dbe-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dbe-174">Request</span></span>

<span data-ttu-id="39dbe-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39dbe-175">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39dbe-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="39dbe-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="39dbe-177">C#</span><span class="sxs-lookup"><span data-stu-id="39dbe-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39dbe-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39dbe-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39dbe-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39dbe-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39dbe-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dbe-180">Response</span></span>

<span data-ttu-id="39dbe-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39dbe-181">The following is an example of the response.</span></span>

> <span data-ttu-id="39dbe-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39dbe-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
