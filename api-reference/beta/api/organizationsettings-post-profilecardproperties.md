---
title: Создание profileCardProperty
description: Используйте этот API для создания нового профиляCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c9b43c3ca76416db4d319fdfcd7631d5eaf3a9b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055591"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="2f905-103">Создание profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="2f905-103">Create profileCardProperty</span></span>

<span data-ttu-id="2f905-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f905-105">Создайте новый [профильCardProperty](../resources/profilecardproperty.md) для организации.</span><span class="sxs-lookup"><span data-stu-id="2f905-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="2f905-106">Новое свойство определено **свойством directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="2f905-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="2f905-107">Дополнительные сведения о добавлении свойств в карточку профилей для организации см. в примере [настройка карточки профиля.](/graph/add-properties-profilecard)</span><span class="sxs-lookup"><span data-stu-id="2f905-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f905-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f905-108">Permissions</span></span>

<span data-ttu-id="2f905-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f905-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f905-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f905-111">Permission type</span></span>                        | <span data-ttu-id="2f905-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f905-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f905-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f905-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f905-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f905-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2f905-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f905-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f905-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f905-116">Not supported.</span></span>                              |
| <span data-ttu-id="2f905-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f905-117">Application</span></span>                            | <span data-ttu-id="2f905-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f905-118">Not supported.</span></span>                              |

><span data-ttu-id="2f905-119">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="2f905-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f905-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f905-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="2f905-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f905-121">Request headers</span></span>

| <span data-ttu-id="2f905-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2f905-122">Name</span></span>          |<span data-ttu-id="2f905-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2f905-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="2f905-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f905-124">Authorization</span></span> | <span data-ttu-id="2f905-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f905-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2f905-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f905-127">Content-Type</span></span>  | <span data-ttu-id="2f905-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f905-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f905-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f905-130">Request body</span></span>

<span data-ttu-id="2f905-131">В корпусе запроса поставляем представление JSON объекта [profileCardProperty.](../resources/profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2f905-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f905-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f905-132">Response</span></span>

<span data-ttu-id="2f905-133">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект profileCardProperty](../resources/profilecardproperty.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2f905-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f905-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f905-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f905-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f905-135">Request</span></span>

<span data-ttu-id="2f905-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f905-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f905-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f905-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="2f905-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f905-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2f905-139">C#</span><span class="sxs-lookup"><span data-stu-id="2f905-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-profilecardproperty-from-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f905-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f905-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-profilecardproperty-from-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f905-141">Java</span><span class="sxs-lookup"><span data-stu-id="2f905-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-profilecardproperty-from-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f905-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f905-142">Response</span></span>

<span data-ttu-id="2f905-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f905-143">The following is an example of the response.</span></span>

> <span data-ttu-id="2f905-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2f905-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


