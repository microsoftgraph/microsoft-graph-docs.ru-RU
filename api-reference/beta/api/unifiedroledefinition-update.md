---
title: Обновление Унифиедроледефинитион
description: Обновление свойств объекта Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb1cd8a7e8cbef279c5007b3cd721193ff25e518
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218943"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="d31e4-103">Обновление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="d31e4-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="d31e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d31e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d31e4-105">Обновление свойств объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d31e4-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d31e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d31e4-106">Permissions</span></span>

<span data-ttu-id="d31e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d31e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d31e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d31e4-109">Permission type</span></span>                        | <span data-ttu-id="d31e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d31e4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d31e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d31e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d31e4-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="d31e4-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="d31e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d31e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d31e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d31e4-114">Not supported.</span></span> |
| <span data-ttu-id="d31e4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d31e4-115">Application</span></span>                            | <span data-ttu-id="d31e4-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="d31e4-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d31e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d31e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d31e4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d31e4-118">Request headers</span></span>

| <span data-ttu-id="d31e4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d31e4-119">Name</span></span>       | <span data-ttu-id="d31e4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d31e4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d31e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d31e4-121">Authorization</span></span> | <span data-ttu-id="d31e4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d31e4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d31e4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d31e4-123">Request body</span></span>

<span data-ttu-id="d31e4-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d31e4-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d31e4-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d31e4-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d31e4-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d31e4-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d31e4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d31e4-127">Property</span></span>     | <span data-ttu-id="d31e4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d31e4-128">Type</span></span>        | <span data-ttu-id="d31e4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d31e4-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d31e4-130">description</span><span class="sxs-lookup"><span data-stu-id="d31e4-130">description</span></span>|<span data-ttu-id="d31e4-131">String</span><span class="sxs-lookup"><span data-stu-id="d31e4-131">String</span></span>| <span data-ttu-id="d31e4-132">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="d31e4-132">The description for the role definition.</span></span> <span data-ttu-id="d31e4-133">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="d31e4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d31e4-134">displayName</span></span>|<span data-ttu-id="d31e4-135">Строка</span><span class="sxs-lookup"><span data-stu-id="d31e4-135">String</span></span>| <span data-ttu-id="d31e4-136">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="d31e4-136">The display name for the role definition.</span></span> <span data-ttu-id="d31e4-137">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="d31e4-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d31e4-138">Required.</span></span>|
|<span data-ttu-id="d31e4-139">id</span><span class="sxs-lookup"><span data-stu-id="d31e4-139">id</span></span>|<span data-ttu-id="d31e4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d31e4-140">String</span></span>| <span data-ttu-id="d31e4-141">Уникальный идентификатор для определения роли.</span><span class="sxs-lookup"><span data-stu-id="d31e4-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="d31e4-142">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d31e4-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="d31e4-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d31e4-143">isBuiltIn</span></span>|<span data-ttu-id="d31e4-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d31e4-144">Boolean</span></span>| <span data-ttu-id="d31e4-145">Флаг, указывающий, является ли определение роли частью набора по умолчанию, входящего в состав продукта или настраиваемого.</span><span class="sxs-lookup"><span data-stu-id="d31e4-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="d31e4-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d31e4-146">Read-only.</span></span> |
|<span data-ttu-id="d31e4-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d31e4-147">isEnabled</span></span>|<span data-ttu-id="d31e4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d31e4-148">Boolean</span></span>| <span data-ttu-id="d31e4-149">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="d31e4-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="d31e4-150">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="d31e4-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="d31e4-151">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="d31e4-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d31e4-152">resourceScopes</span></span>|<span data-ttu-id="d31e4-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d31e4-153">String collection</span></span>| <span data-ttu-id="d31e4-154">Список разрешений областей, к которым применяется определение роли.</span><span class="sxs-lookup"><span data-stu-id="d31e4-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="d31e4-155">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="d31e4-155">Currently only "/" is supported.</span></span> <span data-ttu-id="d31e4-156">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="d31e4-157">**НЕ ИСПОЛЬЗУЙТЕ. Это свойство будет нерекомендуемым в ближайшее время. Присоединение области к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="d31e4-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="d31e4-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d31e4-158">rolePermissions</span></span>|<span data-ttu-id="d31e4-159">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d31e4-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="d31e4-160">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="d31e4-160">List of permissions included in the role.</span></span> <span data-ttu-id="d31e4-161">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="d31e4-162">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="d31e4-162">Required.</span></span> |
|<span data-ttu-id="d31e4-163">templateId</span><span class="sxs-lookup"><span data-stu-id="d31e4-163">templateId</span></span>|<span data-ttu-id="d31e4-164">Строка</span><span class="sxs-lookup"><span data-stu-id="d31e4-164">String</span></span>| <span data-ttu-id="d31e4-165">Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false.</span><span class="sxs-lookup"><span data-stu-id="d31e4-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="d31e4-166">Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов.</span><span class="sxs-lookup"><span data-stu-id="d31e4-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="d31e4-167">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="d31e4-168">version</span><span class="sxs-lookup"><span data-stu-id="d31e4-168">version</span></span>|<span data-ttu-id="d31e4-169">String</span><span class="sxs-lookup"><span data-stu-id="d31e4-169">String</span></span>| <span data-ttu-id="d31e4-170">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="d31e4-170">Indicates version of the role definition.</span></span> <span data-ttu-id="d31e4-171">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d31e4-171">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="d31e4-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d31e4-172">Response</span></span>

<span data-ttu-id="d31e4-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d31e4-173">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d31e4-174">Пример</span><span class="sxs-lookup"><span data-stu-id="d31e4-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="d31e4-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="d31e4-175">Request</span></span>

<span data-ttu-id="d31e4-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d31e4-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d31e4-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="d31e4-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d31e4-178">C#</span><span class="sxs-lookup"><span data-stu-id="d31e4-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d31e4-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d31e4-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d31e4-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d31e4-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d31e4-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="d31e4-181">Response</span></span>

<span data-ttu-id="d31e4-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d31e4-182">The following is an example of the response.</span></span>
> <span data-ttu-id="d31e4-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d31e4-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
