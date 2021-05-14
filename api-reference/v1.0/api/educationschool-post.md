---
title: Создание educationSchool
description: Создание нового объекта educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 98da82ad50ba9f1a8c8b5341730aa3b85f6345c0
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474831"
---
# <a name="create-educationschool"></a><span data-ttu-id="f7e68-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="f7e68-103">Create educationSchool</span></span>

<span data-ttu-id="f7e68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e68-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7e68-105">Создание нового [объекта educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f7e68-105">Create a new [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e68-106">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="f7e68-106">Permissions</span></span>

<span data-ttu-id="f7e68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7e68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e68-109">Permission type</span></span>                        | <span data-ttu-id="f7e68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e68-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f7e68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e68-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7e68-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e68-112">Not supported.</span></span>                              |
| <span data-ttu-id="f7e68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e68-114">Not supported.</span></span>                              |
| <span data-ttu-id="f7e68-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7e68-115">Application</span></span>                            | <span data-ttu-id="f7e68-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e68-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="f7e68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e68-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="f7e68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e68-118">Request headers</span></span>

| <span data-ttu-id="f7e68-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f7e68-119">Name</span></span>          | <span data-ttu-id="f7e68-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e68-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="f7e68-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7e68-121">Authorization</span></span> | <span data-ttu-id="f7e68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e68-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f7e68-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7e68-124">Content-Type</span></span>  | <span data-ttu-id="f7e68-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e68-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7e68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7e68-127">Request body</span></span>

<span data-ttu-id="f7e68-128">В теле запроса поставляем представление JSON объекта [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f7e68-128">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="f7e68-129">В следующей таблице показаны свойства, необходимые при создании [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f7e68-129">The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="f7e68-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7e68-130">Property</span></span>             | <span data-ttu-id="f7e68-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e68-131">Type</span></span>                                               | <span data-ttu-id="f7e68-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e68-132">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7e68-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f7e68-133">displayName</span></span>          | <span data-ttu-id="f7e68-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f7e68-134">String</span></span>                                             | <span data-ttu-id="f7e68-135">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e68-135">Display name of the school.</span></span> <span data-ttu-id="f7e68-136">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="f7e68-136">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                           |
| <span data-ttu-id="f7e68-137">description</span><span class="sxs-lookup"><span data-stu-id="f7e68-137">description</span></span>          | <span data-ttu-id="f7e68-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f7e68-138">String</span></span>                                             | <span data-ttu-id="f7e68-139">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e68-139">Description of the school.</span></span> <span data-ttu-id="f7e68-140">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="f7e68-140">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="f7e68-141">externalSource</span><span class="sxs-lookup"><span data-stu-id="f7e68-141">externalSource</span></span>       | <span data-ttu-id="f7e68-142">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="f7e68-142">educationExternalSource</span></span>                            | <span data-ttu-id="f7e68-143">Источник, из которых была создана эта организация.</span><span class="sxs-lookup"><span data-stu-id="f7e68-143">Source where this organization was created from.</span></span> <span data-ttu-id="f7e68-144">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="f7e68-144">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="f7e68-145">Возможные значения: `sis` " вручную.</span><span class="sxs-lookup"><span data-stu-id="f7e68-145">Possible values are: `sis`, \`manual.</span></span> |
| <span data-ttu-id="f7e68-146">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="f7e68-146">externalSourceDetail</span></span> | <span data-ttu-id="f7e68-147">Строка</span><span class="sxs-lookup"><span data-stu-id="f7e68-147">String</span></span>                                             | <span data-ttu-id="f7e68-148">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="f7e68-148">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="f7e68-149">principalEmail</span><span class="sxs-lookup"><span data-stu-id="f7e68-149">principalEmail</span></span>       | <span data-ttu-id="f7e68-150">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-150">String</span></span>                                             | <span data-ttu-id="f7e68-151">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="f7e68-151">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="f7e68-152">principalName</span><span class="sxs-lookup"><span data-stu-id="f7e68-152">principalName</span></span>        | <span data-ttu-id="f7e68-153">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-153">String</span></span>                                             | <span data-ttu-id="f7e68-154">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="f7e68-154">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="f7e68-155">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="f7e68-155">externalPrincipalId</span></span>  | <span data-ttu-id="f7e68-156">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-156">String</span></span>                                             | <span data-ttu-id="f7e68-157">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7e68-157">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="f7e68-158">highestGrade</span><span class="sxs-lookup"><span data-stu-id="f7e68-158">highestGrade</span></span>         | <span data-ttu-id="f7e68-159">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-159">String</span></span>                                             | <span data-ttu-id="f7e68-160">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="f7e68-160">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="f7e68-161">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="f7e68-161">lowestGrade</span></span>          | <span data-ttu-id="f7e68-162">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-162">String</span></span>                                             | <span data-ttu-id="f7e68-163">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="f7e68-163">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="f7e68-164">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="f7e68-164">schoolNumber</span></span>         | <span data-ttu-id="f7e68-165">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-165">String</span></span>                                             | <span data-ttu-id="f7e68-166">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="f7e68-166">School Number.</span></span>                                                                                                                                                       |
| <span data-ttu-id="f7e68-167">externalId</span><span class="sxs-lookup"><span data-stu-id="f7e68-167">externalId</span></span>           | <span data-ttu-id="f7e68-168">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-168">String</span></span>                                             | <span data-ttu-id="f7e68-169">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7e68-169">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="f7e68-170">phone</span><span class="sxs-lookup"><span data-stu-id="f7e68-170">phone</span></span>                | <span data-ttu-id="f7e68-171">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-171">String</span></span>                                             | <span data-ttu-id="f7e68-172">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e68-172">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="f7e68-173">fax</span><span class="sxs-lookup"><span data-stu-id="f7e68-173">fax</span></span>                  | <span data-ttu-id="f7e68-174">String</span><span class="sxs-lookup"><span data-stu-id="f7e68-174">String</span></span>                                             | <span data-ttu-id="f7e68-175">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e68-175">Fax number of school.</span></span>                                                                                                                                                |
| <span data-ttu-id="f7e68-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="f7e68-176">createdBy</span></span>            | [<span data-ttu-id="f7e68-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7e68-177">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="f7e68-178">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="f7e68-178">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="f7e68-179">address</span><span class="sxs-lookup"><span data-stu-id="f7e68-179">address</span></span>              | [<span data-ttu-id="f7e68-180">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f7e68-180">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="f7e68-181">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f7e68-181">Address of the school.</span></span>                                                                                                                                               |

## <a name="response"></a><span data-ttu-id="f7e68-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e68-182">Response</span></span>

<span data-ttu-id="f7e68-183">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e68-183">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7e68-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7e68-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7e68-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e68-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f7e68-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e68-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-Type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f7e68-187">C#</span><span class="sxs-lookup"><span data-stu-id="f7e68-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7e68-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7e68-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7e68-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7e68-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7e68-190">Java</span><span class="sxs-lookup"><span data-stu-id="f7e68-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7e68-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e68-191">Response</span></span>

> <span data-ttu-id="f7e68-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f7e68-192">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
