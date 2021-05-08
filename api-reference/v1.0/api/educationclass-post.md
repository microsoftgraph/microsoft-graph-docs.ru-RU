---
title: Создание educationClass
description: Создание нового объекта educationClass.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71dcda18e56b6dfd53fa35943e6da246b5b8d68f
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232296"
---
# <a name="create-educationclass"></a><span data-ttu-id="7e8f9-103">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="7e8f9-103">Create educationClass</span></span>

<span data-ttu-id="7e8f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e8f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e8f9-105">Создание нового [объекта educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-105">Create a new [educationClass](../resources/educationclass.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="7e8f9-106">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-106">This will also create a universal group.</span></span> <span data-ttu-id="7e8f9-107">При использовании этого API для создания класса в группу будут добавлены специальные свойства, которые будут добавлять такие функции, как назначения и специальная обработка в Microsoft Teams при создании групп с помощью группы.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-107">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="7e8f9-108">Обратите внимание, что этот API создает только универсальную группу и не создает команду.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-108">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="7e8f9-109">Microsoft Teams предоставляет пользовательский интерфейс для преподавателей для создания групп для своих классов с помощью групп, созданных этим API.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-109">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e8f9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e8f9-110">Permissions</span></span>

<span data-ttu-id="7e8f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e8f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e8f9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e8f9-113">Permission type</span></span>                        | <span data-ttu-id="7e8f9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7e8f9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e8f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-116">Not supported.</span></span>                              |
| <span data-ttu-id="7e8f9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e8f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-118">Not supported.</span></span>                              |
| <span data-ttu-id="7e8f9-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e8f9-119">Application</span></span>                            | <span data-ttu-id="7e8f9-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e8f9-120">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="7e8f9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e8f9-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a><span data-ttu-id="7e8f9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e8f9-122">Request headers</span></span>

| <span data-ttu-id="7e8f9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7e8f9-123">Name</span></span>          | <span data-ttu-id="7e8f9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7e8f9-124">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="7e8f9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e8f9-125">Authorization</span></span> | <span data-ttu-id="7e8f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7e8f9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e8f9-128">Content-Type</span></span>  | <span data-ttu-id="7e8f9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e8f9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e8f9-131">Request body</span></span>

<span data-ttu-id="7e8f9-132">В теле запроса поставляем представление JSON объекта [educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-132">In the request body, supply a JSON representation of the [educationClass](../resources/educationclass.md) object.</span></span>

<span data-ttu-id="7e8f9-133">В следующей таблице показаны свойства, необходимые при создании [educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-133">The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).</span></span>

| <span data-ttu-id="7e8f9-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e8f9-134">Property</span></span>             | <span data-ttu-id="7e8f9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="7e8f9-135">Type</span></span>                                           | <span data-ttu-id="7e8f9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="7e8f9-136">Description</span></span>                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="7e8f9-137">id</span><span class="sxs-lookup"><span data-stu-id="7e8f9-137">id</span></span>                   | <span data-ttu-id="7e8f9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7e8f9-138">String</span></span>                                         | <span data-ttu-id="7e8f9-139">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-139">Object identifier.</span></span> <span data-ttu-id="7e8f9-140">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="7e8f9-140">Inherited from [entity](../resources/entity.md)</span></span> |
| <span data-ttu-id="7e8f9-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7e8f9-141">displayName</span></span>          | <span data-ttu-id="7e8f9-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7e8f9-142">String</span></span>                                         | <span data-ttu-id="7e8f9-143">Название курса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-143">Name of the class.</span></span>                                                 |
| <span data-ttu-id="7e8f9-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7e8f9-144">mailNickname</span></span>         | <span data-ttu-id="7e8f9-145">String</span><span class="sxs-lookup"><span data-stu-id="7e8f9-145">String</span></span>                                         | <span data-ttu-id="7e8f9-146">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-146">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="7e8f9-147">description</span><span class="sxs-lookup"><span data-stu-id="7e8f9-147">description</span></span>          | <span data-ttu-id="7e8f9-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7e8f9-148">String</span></span>                                         | <span data-ttu-id="7e8f9-149">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-149">Description of the class.</span></span>                                          |
| <span data-ttu-id="7e8f9-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="7e8f9-150">createdBy</span></span>            | [<span data-ttu-id="7e8f9-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="7e8f9-151">identitySet</span></span>](../resources/identityset.md)     | <span data-ttu-id="7e8f9-152">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-152">Entity who created the class</span></span>                                       |
| <span data-ttu-id="7e8f9-153">classCode</span><span class="sxs-lookup"><span data-stu-id="7e8f9-153">classCode</span></span>            | <span data-ttu-id="7e8f9-154">String</span><span class="sxs-lookup"><span data-stu-id="7e8f9-154">String</span></span>                                         | <span data-ttu-id="7e8f9-155">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-155">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="7e8f9-156">externalName</span><span class="sxs-lookup"><span data-stu-id="7e8f9-156">externalName</span></span>         | <span data-ttu-id="7e8f9-157">String</span><span class="sxs-lookup"><span data-stu-id="7e8f9-157">String</span></span>                                         | <span data-ttu-id="7e8f9-158">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-158">Name of the class in the syncing system.</span></span>                           |
| <span data-ttu-id="7e8f9-159">externalId</span><span class="sxs-lookup"><span data-stu-id="7e8f9-159">externalId</span></span>           | <span data-ttu-id="7e8f9-160">String</span><span class="sxs-lookup"><span data-stu-id="7e8f9-160">String</span></span>                                         | <span data-ttu-id="7e8f9-161">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-161">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="7e8f9-162">externalSource</span><span class="sxs-lookup"><span data-stu-id="7e8f9-162">externalSource</span></span>       | <span data-ttu-id="7e8f9-163">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="7e8f9-163">educationExternalSource</span></span>                        | <span data-ttu-id="7e8f9-164">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-164">How this class was created.</span></span> <span data-ttu-id="7e8f9-165">Возможные значения: `sis` , `manual`</span><span class="sxs-lookup"><span data-stu-id="7e8f9-165">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="7e8f9-166">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="7e8f9-166">externalSourceDetail</span></span> | <span data-ttu-id="7e8f9-167">Строка</span><span class="sxs-lookup"><span data-stu-id="7e8f9-167">String</span></span>                                         | <span data-ttu-id="7e8f9-168">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-168">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="7e8f9-169">оценка</span><span class="sxs-lookup"><span data-stu-id="7e8f9-169">grade</span></span>                | <span data-ttu-id="7e8f9-170">String</span><span class="sxs-lookup"><span data-stu-id="7e8f9-170">String</span></span>                                         | <span data-ttu-id="7e8f9-171">Уровень класса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-171">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="7e8f9-172">term</span><span class="sxs-lookup"><span data-stu-id="7e8f9-172">term</span></span>                 | [<span data-ttu-id="7e8f9-173">educationTerm</span><span class="sxs-lookup"><span data-stu-id="7e8f9-173">educationTerm</span></span>](../resources/educationterm.md) | <span data-ttu-id="7e8f9-174">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-174">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="7e8f9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e8f9-175">Response</span></span>

<span data-ttu-id="7e8f9-176">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-176">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e8f9-177">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e8f9-177">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e8f9-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e8f9-178">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

### <a name="response"></a><span data-ttu-id="7e8f9-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e8f9-179">Response</span></span>

> <span data-ttu-id="7e8f9-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e8f9-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
