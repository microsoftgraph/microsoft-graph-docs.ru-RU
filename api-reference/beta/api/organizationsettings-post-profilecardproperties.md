---
title: Создание Профилекардпроперти
description: Используйте этот API для создания нового Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fc40b90cf390cc4e996b66bda0929ddd99c824d0
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566661"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="c84a2-103">Создание Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="c84a2-103">Create profileCardProperty</span></span>

<span data-ttu-id="c84a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c84a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c84a2-105">Создание нового [профилекардпроперти](../resources/profilecardproperty.md) для Организации.</span><span class="sxs-lookup"><span data-stu-id="c84a2-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="c84a2-106">Новое свойство определяется свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="c84a2-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="c84a2-107">Дополнительные сведения о добавлении свойств в карточку профиля для организации можно узнать в статье [Настройка карточки профиля](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="c84a2-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="c84a2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c84a2-108">Permissions</span></span>

<span data-ttu-id="c84a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c84a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c84a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c84a2-111">Permission type</span></span>                        | <span data-ttu-id="c84a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c84a2-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c84a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c84a2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c84a2-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c84a2-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c84a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c84a2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c84a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c84a2-116">Not supported.</span></span>                              |
| <span data-ttu-id="c84a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c84a2-117">Application</span></span>                            | <span data-ttu-id="c84a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c84a2-118">Not supported.</span></span>                              |

><span data-ttu-id="c84a2-119">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="c84a2-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="c84a2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c84a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="c84a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c84a2-121">Request headers</span></span>

| <span data-ttu-id="c84a2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c84a2-122">Name</span></span>          |<span data-ttu-id="c84a2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c84a2-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="c84a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c84a2-124">Authorization</span></span> | <span data-ttu-id="c84a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c84a2-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c84a2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c84a2-127">Content-Type</span></span>  | <span data-ttu-id="c84a2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c84a2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c84a2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c84a2-130">Request body</span></span>

<span data-ttu-id="c84a2-131">В тексте запроса добавьте представление объекта [профилекардпроперти](../resources/profilecardproperty.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c84a2-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c84a2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c84a2-132">Response</span></span>

<span data-ttu-id="c84a2-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c84a2-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c84a2-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c84a2-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c84a2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c84a2-135">Request</span></span>

<span data-ttu-id="c84a2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c84a2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c84a2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c84a2-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c84a2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c84a2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c84a2-139">C#</span><span class="sxs-lookup"><span data-stu-id="c84a2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-profilecardproperty-from-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c84a2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c84a2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-profilecardproperty-from-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c84a2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c84a2-141">Response</span></span>

<span data-ttu-id="c84a2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c84a2-142">The following is an example of the response.</span></span>

> <span data-ttu-id="c84a2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c84a2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
