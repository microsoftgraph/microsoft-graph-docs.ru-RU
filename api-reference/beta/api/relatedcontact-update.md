---
title: Update relatedContacts
description: Обновление связанной коллекцииContact объекта educationUser.
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 290901a7a6a04a1d846df3bd423fc3c62c3d5867
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965220"
---
# <a name="update-relatedcontacts"></a><span data-ttu-id="1223e-103">Update relatedContacts</span><span class="sxs-lookup"><span data-stu-id="1223e-103">Update relatedContacts</span></span>

<span data-ttu-id="1223e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1223e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1223e-105">Обновление [связанной коллекцииContact](../resources/relatedContact.md) объекта [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1223e-105">Update the [relatedContact](../resources/relatedContact.md) collection of an [educationUser](../resources/educationuser.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="1223e-106">Обновление **relatedContacts** заменяет всю коллекцию.</span><span class="sxs-lookup"><span data-stu-id="1223e-106">Updating **relatedContacts** replaces the entire collection.</span></span> <span data-ttu-id="1223e-107">Невозможно добавить, удалить или обновить один контакт.</span><span class="sxs-lookup"><span data-stu-id="1223e-107">It is not possible to add, remove, or update a single contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="1223e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1223e-108">Permissions</span></span>

<span data-ttu-id="1223e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1223e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1223e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1223e-111">Permission type</span></span>                        | <span data-ttu-id="1223e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1223e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1223e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1223e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1223e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1223e-114">Not supported.</span></span>                              |
| <span data-ttu-id="1223e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1223e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1223e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1223e-116">Not supported.</span></span>                              |
| <span data-ttu-id="1223e-117">Application</span><span class="sxs-lookup"><span data-stu-id="1223e-117">Application</span></span>                            | <span data-ttu-id="1223e-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1223e-118">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="1223e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1223e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1223e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1223e-120">Request headers</span></span>

| <span data-ttu-id="1223e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1223e-121">Name</span></span>          | <span data-ttu-id="1223e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1223e-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="1223e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1223e-123">Authorization</span></span> | <span data-ttu-id="1223e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1223e-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1223e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1223e-126">Content-Type</span></span>  | <span data-ttu-id="1223e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1223e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1223e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1223e-129">Request body</span></span>

<span data-ttu-id="1223e-130">В теле запроса поставляем представление JSON [связанной коллекцииContact.](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="1223e-130">In the request body, supply a JSON representation of the [relatedContact](../resources/relatedcontact.md) collection.</span></span>

<span data-ttu-id="1223e-131">В следующей таблице показаны свойства, необходимые при обновлении [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1223e-131">The following table shows the properties that are required when you update the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="1223e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1223e-132">Property</span></span>        | <span data-ttu-id="1223e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1223e-133">Type</span></span>                                                        | <span data-ttu-id="1223e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1223e-134">Description</span></span>                                    |
| :-------------- | :---------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="1223e-135">relatedContacts</span><span class="sxs-lookup"><span data-stu-id="1223e-135">relatedContacts</span></span> | <span data-ttu-id="1223e-136">[коллекция relatedContact](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="1223e-136">[relatedContact](../resources/relatedcontact.md) collection</span></span> | <span data-ttu-id="1223e-137">Полный набор связанных контактов для пользователя</span><span class="sxs-lookup"><span data-stu-id="1223e-137">The complete set of related contact for a user</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="1223e-138">Это обновление должно быть отдельной операцией.</span><span class="sxs-lookup"><span data-stu-id="1223e-138">This update must be a distinct operation.</span></span> <span data-ttu-id="1223e-139">Его нельзя сочетать с обновлениями других [свойств educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1223e-139">It cannot be combined with updates to other [educationUser](../resources/educationuser.md) properties.</span></span>
> <span data-ttu-id="1223e-140">Например, для обновления как **связанныхContacts,** так и **displayName** требуется два разных запроса.</span><span class="sxs-lookup"><span data-stu-id="1223e-140">For example, updating both **relatedContacts** and **displayName** requires two distinct requests.</span></span>

## <a name="response"></a><span data-ttu-id="1223e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1223e-141">Response</span></span>

<span data-ttu-id="1223e-142">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationUser](../resources/educationuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1223e-142">If successful, this method returns a `200 OK` response code and an updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1223e-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="1223e-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1223e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1223e-144">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="1223e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1223e-145">Response</span></span>

<span data-ttu-id="1223e-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1223e-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
