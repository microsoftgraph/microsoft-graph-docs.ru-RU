---
title: Создание educationSchool
description: Создание нового объекта educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f9bf1499ef3c1d0106d9daac1bbda8f7ef25926d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232250"
---
# <a name="create-educationschool"></a><span data-ttu-id="6b1c3-103">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="6b1c3-103">Create educationSchool</span></span>

<span data-ttu-id="6b1c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b1c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b1c3-105">Создание нового [объекта educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-105">Create a new [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b1c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b1c3-106">Permissions</span></span>

<span data-ttu-id="6b1c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b1c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b1c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b1c3-109">Permission type</span></span>                        | <span data-ttu-id="6b1c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6b1c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b1c3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-112">Not supported.</span></span>                              |
| <span data-ttu-id="6b1c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b1c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-114">Not supported.</span></span>                              |
| <span data-ttu-id="6b1c3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b1c3-115">Application</span></span>                            | <span data-ttu-id="6b1c3-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b1c3-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="6b1c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b1c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="6b1c3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b1c3-118">Request headers</span></span>

| <span data-ttu-id="6b1c3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b1c3-119">Name</span></span>          | <span data-ttu-id="6b1c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6b1c3-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="6b1c3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b1c3-121">Authorization</span></span> | <span data-ttu-id="6b1c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6b1c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b1c3-124">Content-Type</span></span>  | <span data-ttu-id="6b1c3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b1c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b1c3-127">Request body</span></span>

<span data-ttu-id="6b1c3-128">В теле запроса поставляем представление JSON объекта [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-128">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="6b1c3-129">В следующей таблице показаны свойства, необходимые при создании [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6b1c3-129">The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="6b1c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b1c3-130">Property</span></span>             | <span data-ttu-id="6b1c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6b1c3-131">Type</span></span>                                               | <span data-ttu-id="6b1c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6b1c3-132">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6b1c3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6b1c3-133">displayName</span></span>          | <span data-ttu-id="6b1c3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6b1c3-134">String</span></span>                                             | <span data-ttu-id="6b1c3-135">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-135">Display name of the school.</span></span> <span data-ttu-id="6b1c3-136">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6b1c3-136">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                           |
| <span data-ttu-id="6b1c3-137">description</span><span class="sxs-lookup"><span data-stu-id="6b1c3-137">description</span></span>          | <span data-ttu-id="6b1c3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6b1c3-138">String</span></span>                                             | <span data-ttu-id="6b1c3-139">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-139">Description of the school.</span></span> <span data-ttu-id="6b1c3-140">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6b1c3-140">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="6b1c3-141">externalSource</span><span class="sxs-lookup"><span data-stu-id="6b1c3-141">externalSource</span></span>       | <span data-ttu-id="6b1c3-142">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6b1c3-142">educationExternalSource</span></span>                            | <span data-ttu-id="6b1c3-143">Источник, из которых была создана эта организация.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-143">Source where this organization was created from.</span></span> <span data-ttu-id="6b1c3-144">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6b1c3-144">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="6b1c3-145">Возможные значения: `sis` " вручную.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-145">Possible values are: `sis`, \`manual.</span></span> |
| <span data-ttu-id="6b1c3-146">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="6b1c3-146">externalSourceDetail</span></span> | <span data-ttu-id="6b1c3-147">Строка</span><span class="sxs-lookup"><span data-stu-id="6b1c3-147">String</span></span>                                             | <span data-ttu-id="6b1c3-148">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-148">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="6b1c3-149">principalEmail</span><span class="sxs-lookup"><span data-stu-id="6b1c3-149">principalEmail</span></span>       | <span data-ttu-id="6b1c3-150">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-150">String</span></span>                                             | <span data-ttu-id="6b1c3-151">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-151">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="6b1c3-152">principalName</span><span class="sxs-lookup"><span data-stu-id="6b1c3-152">principalName</span></span>        | <span data-ttu-id="6b1c3-153">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-153">String</span></span>                                             | <span data-ttu-id="6b1c3-154">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-154">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="6b1c3-155">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="6b1c3-155">externalPrincipalId</span></span>  | <span data-ttu-id="6b1c3-156">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-156">String</span></span>                                             | <span data-ttu-id="6b1c3-157">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-157">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="6b1c3-158">highestGrade</span><span class="sxs-lookup"><span data-stu-id="6b1c3-158">highestGrade</span></span>         | <span data-ttu-id="6b1c3-159">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-159">String</span></span>                                             | <span data-ttu-id="6b1c3-160">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-160">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="6b1c3-161">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="6b1c3-161">lowestGrade</span></span>          | <span data-ttu-id="6b1c3-162">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-162">String</span></span>                                             | <span data-ttu-id="6b1c3-163">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-163">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="6b1c3-164">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="6b1c3-164">schoolNumber</span></span>         | <span data-ttu-id="6b1c3-165">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-165">String</span></span>                                             | <span data-ttu-id="6b1c3-166">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-166">School Number.</span></span>                                                                                                                                                       |
| <span data-ttu-id="6b1c3-167">externalId</span><span class="sxs-lookup"><span data-stu-id="6b1c3-167">externalId</span></span>           | <span data-ttu-id="6b1c3-168">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-168">String</span></span>                                             | <span data-ttu-id="6b1c3-169">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-169">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="6b1c3-170">phone</span><span class="sxs-lookup"><span data-stu-id="6b1c3-170">phone</span></span>                | <span data-ttu-id="6b1c3-171">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-171">String</span></span>                                             | <span data-ttu-id="6b1c3-172">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-172">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="6b1c3-173">fax</span><span class="sxs-lookup"><span data-stu-id="6b1c3-173">fax</span></span>                  | <span data-ttu-id="6b1c3-174">String</span><span class="sxs-lookup"><span data-stu-id="6b1c3-174">String</span></span>                                             | <span data-ttu-id="6b1c3-175">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-175">Fax number of school.</span></span>                                                                                                                                                |
| <span data-ttu-id="6b1c3-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="6b1c3-176">createdBy</span></span>            | [<span data-ttu-id="6b1c3-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b1c3-177">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="6b1c3-178">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-178">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="6b1c3-179">address</span><span class="sxs-lookup"><span data-stu-id="6b1c3-179">address</span></span>              | [<span data-ttu-id="6b1c3-180">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6b1c3-180">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="6b1c3-181">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-181">Address of the school.</span></span>                                                                                                                                               |

## <a name="response"></a><span data-ttu-id="6b1c3-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b1c3-182">Response</span></span>

<span data-ttu-id="6b1c3-183">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-183">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b1c3-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b1c3-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b1c3-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b1c3-185">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="6b1c3-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b1c3-186">Response</span></span>

> <span data-ttu-id="6b1c3-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b1c3-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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
