---
title: Update relatedContacts
description: Обновление связанной коллекцииContact объекта educationUser.
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f6217c1ea0859de21fa70c53810e825327d497f2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200918"
---
# <a name="update-relatedcontacts"></a><span data-ttu-id="b0321-103">Update relatedContacts</span><span class="sxs-lookup"><span data-stu-id="b0321-103">Update relatedContacts</span></span>

<span data-ttu-id="b0321-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0321-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0321-105">Обновление [связанной коллекцииContact](../resources/relatedContact.md) объекта [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b0321-105">Update the [relatedContact](../resources/relatedContact.md) collection of an [educationUser](../resources/educationuser.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="b0321-106">Обновление **relatedContacts** заменяет всю коллекцию.</span><span class="sxs-lookup"><span data-stu-id="b0321-106">Updating **relatedContacts** replaces the entire collection.</span></span> <span data-ttu-id="b0321-107">Невозможно добавить, удалить или обновить один контакт.</span><span class="sxs-lookup"><span data-stu-id="b0321-107">It is not possible to add, remove, or update a single contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0321-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0321-108">Permissions</span></span>

<span data-ttu-id="b0321-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0321-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0321-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0321-111">Permission type</span></span>                        | <span data-ttu-id="b0321-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0321-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b0321-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0321-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0321-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0321-114">Not supported.</span></span>                              |
| <span data-ttu-id="b0321-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0321-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0321-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0321-116">Not supported.</span></span>                              |
| <span data-ttu-id="b0321-117">Application</span><span class="sxs-lookup"><span data-stu-id="b0321-117">Application</span></span>                            | <span data-ttu-id="b0321-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0321-118">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="b0321-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0321-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0321-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0321-120">Request headers</span></span>

| <span data-ttu-id="b0321-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0321-121">Name</span></span>          | <span data-ttu-id="b0321-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0321-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="b0321-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0321-123">Authorization</span></span> | <span data-ttu-id="b0321-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0321-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b0321-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0321-126">Content-Type</span></span>  | <span data-ttu-id="b0321-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0321-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0321-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0321-129">Request body</span></span>

<span data-ttu-id="b0321-130">В теле запроса поставляем представление JSON [связанной коллекцииContact.](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="b0321-130">In the request body, supply a JSON representation of the [relatedContact](../resources/relatedcontact.md) collection.</span></span>

<span data-ttu-id="b0321-131">В следующей таблице показаны свойства, необходимые при обновлении [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b0321-131">The following table shows the properties that are required when you update the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="b0321-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0321-132">Property</span></span>        | <span data-ttu-id="b0321-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b0321-133">Type</span></span>                                                        | <span data-ttu-id="b0321-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b0321-134">Description</span></span>                                    |
| :-------------- | :---------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="b0321-135">relatedContacts</span><span class="sxs-lookup"><span data-stu-id="b0321-135">relatedContacts</span></span> | <span data-ttu-id="b0321-136">[коллекция relatedContact](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="b0321-136">[relatedContact](../resources/relatedcontact.md) collection</span></span> | <span data-ttu-id="b0321-137">Полный набор связанных контактов для пользователя</span><span class="sxs-lookup"><span data-stu-id="b0321-137">The complete set of related contact for a user</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="b0321-138">Это обновление должно быть отдельной операцией.</span><span class="sxs-lookup"><span data-stu-id="b0321-138">This update must be a distinct operation.</span></span> <span data-ttu-id="b0321-139">Его нельзя сочетать с обновлениями других [свойств educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b0321-139">It cannot be combined with updates to other [educationUser](../resources/educationuser.md) properties.</span></span>
> <span data-ttu-id="b0321-140">Например, для обновления как **связанныхContacts,** так и **displayName** требуется два разных запроса.</span><span class="sxs-lookup"><span data-stu-id="b0321-140">For example, updating both **relatedContacts** and **displayName** requires two distinct requests.</span></span>

## <a name="response"></a><span data-ttu-id="b0321-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0321-141">Response</span></span>

<span data-ttu-id="b0321-142">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationUser](../resources/educationuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0321-142">If successful, this method returns a `200 OK` response code and an updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0321-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0321-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0321-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0321-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b0321-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0321-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}
-->

```http
PATCH https://graph.microsoft.com/beta/education/users/{educationUserId}
Content-Type: application/json
Content-length: 408

{
  "relatedContacts": [
    {
      "displayName": "Father Time",
      "emailAddress": "father@time.com",
      "mobilePhone": "4251231234",
      "relationship": "guardian",
      "accessConsent": true
    },
    {
      "displayName": "Mother Nature",
      "emailAddress": "mother@nature.co.uk",
      "mobilePhone": "3251231234",
      "relationship": "parent",
      "accessConsent": true
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b0321-146">C#</span><span class="sxs-lookup"><span data-stu-id="b0321-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0321-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0321-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0321-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0321-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0321-149">Java</span><span class="sxs-lookup"><span data-stu-id="b0321-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0321-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0321-150">Response</span></span>

<span data-ttu-id="b0321-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0321-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "4b712dc5-2dc5-4b71-c52d-714bc52d714b",
  "relatedContacts": [
      {
          "displayName": "Father Time",
          "emailAddress": "father@time.com",
          "mobilePhone": "4251231234",
          "relationship": "guardian",
          "accessConsent": true
      },
      {
          "displayName": "Mother Nature",
          "emailAddress": "mother@nature.co.uk",
          "mobilePhone": "3251231234",
          "relationship": "parent",
          "accessConsent": true
      }
  ]
}
```
