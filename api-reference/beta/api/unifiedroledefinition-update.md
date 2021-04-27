---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0e7c38a8f388492fd4ca079993419d566f7ad8d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053400"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="26878-103">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="26878-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="26878-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26878-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26878-105">Обновление свойств объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="26878-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26878-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26878-106">Permissions</span></span>

<span data-ttu-id="26878-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26878-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26878-109">Permission type</span></span>                        | <span data-ttu-id="26878-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26878-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26878-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26878-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26878-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="26878-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="26878-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26878-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26878-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26878-114">Not supported.</span></span> |
| <span data-ttu-id="26878-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="26878-115">Application</span></span>                            | <span data-ttu-id="26878-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="26878-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="26878-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26878-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26878-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26878-118">Request headers</span></span>

| <span data-ttu-id="26878-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26878-119">Name</span></span>       | <span data-ttu-id="26878-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26878-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26878-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26878-121">Authorization</span></span> | <span data-ttu-id="26878-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="26878-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26878-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26878-123">Request body</span></span>

<span data-ttu-id="26878-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="26878-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="26878-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="26878-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26878-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="26878-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26878-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="26878-127">Property</span></span>     | <span data-ttu-id="26878-128">Тип</span><span class="sxs-lookup"><span data-stu-id="26878-128">Type</span></span>        | <span data-ttu-id="26878-129">Описание</span><span class="sxs-lookup"><span data-stu-id="26878-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26878-130">description</span><span class="sxs-lookup"><span data-stu-id="26878-130">description</span></span>|<span data-ttu-id="26878-131">String</span><span class="sxs-lookup"><span data-stu-id="26878-131">String</span></span>| <span data-ttu-id="26878-132">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="26878-132">The description for the role definition.</span></span> <span data-ttu-id="26878-133">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="26878-134">displayName</span><span class="sxs-lookup"><span data-stu-id="26878-134">displayName</span></span>|<span data-ttu-id="26878-135">String</span><span class="sxs-lookup"><span data-stu-id="26878-135">String</span></span>| <span data-ttu-id="26878-136">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="26878-136">The display name for the role definition.</span></span> <span data-ttu-id="26878-137">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="26878-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26878-138">Required.</span></span>|
|<span data-ttu-id="26878-139">id</span><span class="sxs-lookup"><span data-stu-id="26878-139">id</span></span>|<span data-ttu-id="26878-140">String</span><span class="sxs-lookup"><span data-stu-id="26878-140">String</span></span>| <span data-ttu-id="26878-141">Уникальный идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="26878-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="26878-142">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="26878-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="26878-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="26878-143">isBuiltIn</span></span>|<span data-ttu-id="26878-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="26878-144">Boolean</span></span>| <span data-ttu-id="26878-145">Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="26878-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="26878-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26878-146">Read-only.</span></span> |
|<span data-ttu-id="26878-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="26878-147">isEnabled</span></span>|<span data-ttu-id="26878-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="26878-148">Boolean</span></span>| <span data-ttu-id="26878-149">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="26878-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="26878-150">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="26878-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="26878-151">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="26878-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="26878-152">resourceScopes</span></span>|<span data-ttu-id="26878-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26878-153">String collection</span></span>| <span data-ttu-id="26878-154">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="26878-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="26878-155">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="26878-155">Currently only "/" is supported.</span></span> <span data-ttu-id="26878-156">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="26878-157">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="26878-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="26878-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="26878-158">rolePermissions</span></span>|<span data-ttu-id="26878-159">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="26878-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="26878-160">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="26878-160">List of permissions included in the role.</span></span> <span data-ttu-id="26878-161">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="26878-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26878-162">Required.</span></span> |
|<span data-ttu-id="26878-163">templateId</span><span class="sxs-lookup"><span data-stu-id="26878-163">templateId</span></span>|<span data-ttu-id="26878-164">String</span><span class="sxs-lookup"><span data-stu-id="26878-164">String</span></span>| <span data-ttu-id="26878-165">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="26878-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="26878-166">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="26878-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="26878-167">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="26878-168">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="26878-168">inheritsPermissionsFrom</span></span>| <span data-ttu-id="26878-169">[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="26878-169">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="26878-170">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="26878-170">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="26878-171">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="26878-171">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="26878-172">version</span><span class="sxs-lookup"><span data-stu-id="26878-172">version</span></span>|<span data-ttu-id="26878-173">String</span><span class="sxs-lookup"><span data-stu-id="26878-173">String</span></span>| <span data-ttu-id="26878-174">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="26878-174">Indicates version of the role definition.</span></span> <span data-ttu-id="26878-175">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="26878-175">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="26878-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="26878-176">Response</span></span>

<span data-ttu-id="26878-177">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26878-177">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26878-178">Пример</span><span class="sxs-lookup"><span data-stu-id="26878-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="26878-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="26878-179">Request</span></span>

<span data-ttu-id="26878-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26878-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26878-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="26878-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26878-182">C#</span><span class="sxs-lookup"><span data-stu-id="26878-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26878-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26878-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26878-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26878-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26878-185">Java</span><span class="sxs-lookup"><span data-stu-id="26878-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26878-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="26878-186">Response</span></span>

<span data-ttu-id="26878-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26878-187">The following is an example of the response.</span></span>
> <span data-ttu-id="26878-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26878-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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


