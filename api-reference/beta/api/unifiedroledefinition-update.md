---
title: Обновление Унифиедроледефинитион
description: Обновление свойств объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd76b6baa201315dc21ae5b8f610f6c58233b37f
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437757"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="97bd9-103">Обновление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="97bd9-103">Update unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97bd9-104">Обновление свойств объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="97bd9-104">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97bd9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97bd9-105">Permissions</span></span>

<span data-ttu-id="97bd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97bd9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97bd9-108">Permission type</span></span>                        | <span data-ttu-id="97bd9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97bd9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97bd9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97bd9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97bd9-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="97bd9-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="97bd9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97bd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97bd9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97bd9-113">Not supported.</span></span> |
| <span data-ttu-id="97bd9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97bd9-114">Application</span></span>                            | <span data-ttu-id="97bd9-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="97bd9-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="97bd9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97bd9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97bd9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97bd9-117">Request headers</span></span>

| <span data-ttu-id="97bd9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="97bd9-118">Name</span></span>       | <span data-ttu-id="97bd9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="97bd9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97bd9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97bd9-120">Authorization</span></span> | <span data-ttu-id="97bd9-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="97bd9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="97bd9-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97bd9-122">Request body</span></span>

<span data-ttu-id="97bd9-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="97bd9-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="97bd9-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="97bd9-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="97bd9-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="97bd9-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97bd9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="97bd9-126">Property</span></span>     | <span data-ttu-id="97bd9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="97bd9-127">Type</span></span>        | <span data-ttu-id="97bd9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="97bd9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97bd9-129">description</span><span class="sxs-lookup"><span data-stu-id="97bd9-129">description</span></span>|<span data-ttu-id="97bd9-130">String</span><span class="sxs-lookup"><span data-stu-id="97bd9-130">String</span></span>| <span data-ttu-id="97bd9-131">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="97bd9-131">The description for the role definition.</span></span> <span data-ttu-id="97bd9-132">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="97bd9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="97bd9-133">displayName</span></span>|<span data-ttu-id="97bd9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="97bd9-134">String</span></span>| <span data-ttu-id="97bd9-135">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="97bd9-135">The display name for the role definition.</span></span> <span data-ttu-id="97bd9-136">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="97bd9-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97bd9-137">Required.</span></span>|
|<span data-ttu-id="97bd9-138">id</span><span class="sxs-lookup"><span data-stu-id="97bd9-138">id</span></span>|<span data-ttu-id="97bd9-139">String</span><span class="sxs-lookup"><span data-stu-id="97bd9-139">String</span></span>| <span data-ttu-id="97bd9-140">Уникальный идентификатор для определения роли.</span><span class="sxs-lookup"><span data-stu-id="97bd9-140">The unique identifier for the role definition.</span></span> <span data-ttu-id="97bd9-141">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97bd9-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="97bd9-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="97bd9-142">isBuiltIn</span></span>|<span data-ttu-id="97bd9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="97bd9-143">Boolean</span></span>| <span data-ttu-id="97bd9-144">Флаг, указывающий, является ли определение роли частью набора по умолчанию, входящего в состав продукта или настраиваемого.</span><span class="sxs-lookup"><span data-stu-id="97bd9-144">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="97bd9-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97bd9-145">Read-only.</span></span> |
|<span data-ttu-id="97bd9-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="97bd9-146">isEnabled</span></span>|<span data-ttu-id="97bd9-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="97bd9-147">Boolean</span></span>| <span data-ttu-id="97bd9-148">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="97bd9-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="97bd9-149">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="97bd9-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="97bd9-150">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="97bd9-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="97bd9-151">resourceScopes</span></span>|<span data-ttu-id="97bd9-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="97bd9-152">String collection</span></span>| <span data-ttu-id="97bd9-153">Список разрешений областей, к которым применяется определение роли.</span><span class="sxs-lookup"><span data-stu-id="97bd9-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="97bd9-154">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="97bd9-154">Currently only "/" is supported.</span></span> <span data-ttu-id="97bd9-155">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-155">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="97bd9-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="97bd9-156">rolePermissions</span></span>|<span data-ttu-id="97bd9-157">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="97bd9-157">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="97bd9-158">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="97bd9-158">List of permissions included in the role.</span></span> <span data-ttu-id="97bd9-159">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-159">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="97bd9-160">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="97bd9-160">Required.</span></span> |
|<span data-ttu-id="97bd9-161">templateId</span><span class="sxs-lookup"><span data-stu-id="97bd9-161">templateId</span></span>|<span data-ttu-id="97bd9-162">String</span><span class="sxs-lookup"><span data-stu-id="97bd9-162">String</span></span>| <span data-ttu-id="97bd9-163">Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false.</span><span class="sxs-lookup"><span data-stu-id="97bd9-163">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="97bd9-164">Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов.</span><span class="sxs-lookup"><span data-stu-id="97bd9-164">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="97bd9-165">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-165">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="97bd9-166">version</span><span class="sxs-lookup"><span data-stu-id="97bd9-166">version</span></span>|<span data-ttu-id="97bd9-167">String</span><span class="sxs-lookup"><span data-stu-id="97bd9-167">String</span></span>| <span data-ttu-id="97bd9-168">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="97bd9-168">Indicates version of the role definition.</span></span> <span data-ttu-id="97bd9-169">Только для чтения, если для Builtin задано значение true.</span><span class="sxs-lookup"><span data-stu-id="97bd9-169">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="97bd9-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="97bd9-170">Response</span></span>

<span data-ttu-id="97bd9-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97bd9-171">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97bd9-172">Пример</span><span class="sxs-lookup"><span data-stu-id="97bd9-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="97bd9-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="97bd9-173">Request</span></span>

<span data-ttu-id="97bd9-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97bd9-174">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97bd9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="97bd9-175">Response</span></span>

<span data-ttu-id="97bd9-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97bd9-176">The following is an example of the response.</span></span>

> <span data-ttu-id="97bd9-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97bd9-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
